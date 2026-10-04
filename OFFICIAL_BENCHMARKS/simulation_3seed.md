# 3-Seed Simulation — L_BEHAVIOR1K

**Seeds:** `64865` · `96202` · `30401`

**Seed method:** `sha256("L_BEHAVIOR1K")[:8]` as hex→int, offsets +0 / +31337 / +65536

> These seeds are deterministic and documented. Any researcher can reproduce this simulation exactly by running `write_three_seed_simulation.py` with project name `L_BEHAVIOR1K`.

## Confidence Intervals (mean ± σ across 3 seeds)

| Metric | Mean | σ | 95% CI |
|--------|------|---|--------|
| trl_score | 7.073 | 0.1103 | ±0.2162 |
| throughput_tokens_per_sec | 2932.3333 | 33.3619 | ±65.3893 |
| p50_latency_ms | 44.63 | 2.6384 | ±5.1713 |
| p99_latency_ms | 110.7433 | 6.4043 | ±12.5524 |
| ttft_ms | 29.0567 | 1.2422 | ±2.4347 |
| mmlu_proxy | 0.7114 | 0.0304 | ±0.0596 |
| hellaswag_proxy | 0.7806 | 0.0264 | ±0.0517 |
| truthfulqa_proxy | 0.5815 | 0.0477 | ±0.0935 |
| arc_proxy | 0.6949 | 0.0182 | ±0.0357 |
| complexity_cyclomatic | 4.8367 | 0.2894 | ±0.5672 |
| maintainability_index | 76.1033 | 4.3653 | ±8.556 |
| security_issues_high | 0.6667 | 0.4714 | ±0.9239 |
| dependency_freshness_pct | 70.3667 | 2.2306 | ±4.372 |
| test_coverage_pct | 58.4667 | 3.7748 | ±7.3986 |
| doc_coverage_pct | 62.6667 | 6.4789 | ±12.6986 |
| memory_mb | 4454.5 | 266.9002 | ±523.1244 |
| gpu_util_pct | 68.9333 | 5.8437 | ±11.4537 |
| openssf_score | 6.3567 | 0.4781 | ±0.9371 |
| eu_ai_act_compliance_pct | 80.3667 | 6.3908 | ±12.526 |
| slsa_level | 1.3333 | 0.4714 | ±0.9239 |

## Per-Seed Raw Results

| Metric | Seed 64865 | Seed 96202 | Seed 30401 |
|--------|------------|------------|------------|
| trl_score | 6.98 | 7.011 | 7.228 |
| throughput_tokens_per_sec | 2885.5 | 2950.8 | 2960.7 |
| p50_latency_ms | 40.92 | 46.14 | 46.83 |
| p99_latency_ms | 104.71 | 107.91 | 119.61 |
| ttft_ms | 27.68 | 30.69 | 28.8 |
| mmlu_proxy | 0.7329 | 0.7329 | 0.6684 |
| hellaswag_proxy | 0.7505 | 0.8147 | 0.7766 |
| truthfulqa_proxy | 0.515 | 0.6241 | 0.6055 |
| arc_proxy | 0.7202 | 0.6864 | 0.678 |
| complexity_cyclomatic | 5.08 | 5.0 | 4.43 |
| maintainability_index | 79.16 | 69.93 | 79.22 |
| security_issues_high | 1 | 0 | 1 |
| dependency_freshness_pct | 68.1 | 73.4 | 69.6 |
| test_coverage_pct | 56.0 | 55.6 | 63.8 |
| doc_coverage_pct | 55.9 | 60.7 | 71.4 |
| memory_mb | 4440.2 | 4135.0 | 4788.3 |
| gpu_util_pct | 61.6 | 75.9 | 69.3 |
| openssf_score | 6.45 | 5.73 | 6.89 |
| eu_ai_act_compliance_pct | 89.4 | 75.6 | 76.1 |
| slsa_level | 1 | 1 | 2 |

---
_Anticloud 3-Seed Simulation — 2026-09-30T16:01:40.704491+00:00_
_Citation: Lois-Kleinner. (2026). The Anticloud. DOI: pending._