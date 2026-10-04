# Deploy Guide — L_BEHAVIOR1K
**Tier:** TIER_5_WORLD_NEURO_EMBODIED | **Stack:** Python 3.11, OmniGibson (simulation), PyTorch 2.10+, PAX 27B, AIOSS_FORMAT
**Air-gap capable after initial setup.**

## Prerequisites
Python 3.11+, OmniGibson simulator (separate install), PyTorch 2.10+, A100 GPU for fast sim.

## Environment
A100 80GB for parallel simulation. OmniGibson requires NVIDIA Omniverse. 64GB RAM.

## AIOSS Integration
```bash
aioss init --module L_BEHAVIOR1K --output ./l_behavior1k.aioss
aioss append --chain ./l_behavior1k.aioss --payload ./output.bin --module L_BEHAVIOR1K
aioss verify --chain ./l_behavior1k.aioss
```

## Air-Gap Setup
```bash
pip download -r requirements.txt -d ./wheels/
pip install --no-index --find-links ./wheels/ -r requirements.txt
```

## PAX 27B Harness Wiring
```python
from anticloud_pax import PAXHarness
harness = PAXHarness(
    model_path="./pax-27b-q4.gguf",
    module="L_BEHAVIOR1K",
    aioss_chain="./L_BEHAVIOR1K.aioss",
    classification="L5_NARROW_L2_GENERAL"
)
result = harness.process(input_data)
```

## Verification
```bash
aioss verify --chain ./L_BEHAVIOR1K.aioss --verbose
python -m L_BEHAVIOR1K.tests.smoke
```
