# Developer Cookbook — L_BEHAVIOR1K
**Stack:** Python 3.11, OmniGibson (simulation), PyTorch 2.10+, PAX 27B, AIOSS_FORMAT
**Domain:** BEHAVIOR-1K: 1000-task embodied AI benchmark suite for Anticloud robot agents

## Run BEHAVIOR-1K evaluation
```python
from l_behavior1k import BehaviorBenchmark

bench = BehaviorBenchmark(
    agent_policy="./anticloud_robot_policy.pt",
    pax_model="./pax-27b-q4.gguf",
    n_tasks=1000,
    aioss_chain="./behavior1k.aioss"
)

results = bench.run(parallel_envs=8)
print(f"Overall success rate: {results.overall_success:.2%}")
print(f"Top-5 failed tasks: {results.most_failed_tasks[:5]}")
print(f"AIOSS certified score: {results.chain_hash}")
```

## AIOSS Chain Append
```python
import hashlib, time

def aioss_append(chain_path, payload: bytes, module_id: str):
    entry_hash = hashlib.sha3_256(payload).digest()
    ts = int(time.time_ns()).to_bytes(8, 'big')
    with open(chain_path, 'rb') as f:
        f.seek(-32, 2); prev_hash = f.read(32)
    new_hash = hashlib.sha3_256(prev_hash + entry_hash + ts).digest()
    with open(chain_path, 'ab') as f:
        f.write(ts + entry_hash + new_hash)
    return new_hash.hex()
```
