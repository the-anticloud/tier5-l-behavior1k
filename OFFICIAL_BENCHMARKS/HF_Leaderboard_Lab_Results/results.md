# HF_Leaderboard_Lab_Results

**Project:** `L_BEHAVIOR1K`  
**Tier:** `TIER_5_WORLD_NEURO_EMBODIED`  
**Slug:** `StanfordVL/BEHAVIOR-1K`  
**Commit:** `bd049de3119a`  
**Run:** `2026-09-30T15:07:07.146295+00:00`  

## Isolation Environment

| Field | Value |
| ----- | ----- |
| Platform | `win32` |
| Python | `3.12.10` |
| HF model | `distilbert-base-uncased` |
| HF load time | `4.42s` |
| Inference device | `cpu` |

## Results

**Framework:** [HuggingFace Open LLM Leaderboard (proxy via distilbert-base-uncased)](https://huggingface.co/docs/leaderboards/en/open_llm_leaderboard/archive)

**Model used:** `distilbert-base-uncased`

### Inference Latency (Classification)

| Metric | Value |
| ------ | ----- |
| Avg latency | **51.34 ms** |
| Min latency | 40.45 ms |
| Max latency | 61.06 ms |
| Samples | 5 |

### Real Tokenization Results

| Field | Value |
| ----- | ----- |
| Token count | **38** |
| Tokenization latency | 1.0 ms |
| Classification label | `LABEL_0` |
| Classification score | 0.5898 |
| Classification latency | 95.97 ms |
| Status | **PASS** |

**Input text tokenized:**
```
L_BEHAVIOR1K (StanfordVL/BEHAVIOR-1K) — 4078 files, 166918 source lines, licence MIT, primary language ['Python']
```

**First 20 tokens:**
```
['[CLS]', 'l', '_', 'behavior', '##1', '##k', '(', 'stanford', '##v', '##l', '/', 'behavior', '-', '1', '##k', ')', '—', '407', '##8', 'files']
```

> Full MMLU/HellaSwag/TruthfulQA/ARC/Winogrande/GSM8K require dedicated GPU.
> These results are CPU inference proxy metrics using distilbert-base-uncased.

---
_Anticloud Benchmark Suite — isolation log — 2026-09-30T15:07:07.146295+00:00_