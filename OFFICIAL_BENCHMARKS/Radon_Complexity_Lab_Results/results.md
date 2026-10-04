# Radon_Complexity_Lab_Results
**Project:** `L_BEHAVIOR1K` | **Status:** `PASS` | **Run:** `2026-09-30T17:14:20.030944+00:00`

**Framework:** [Radon — Cyclomatic Complexity & Maintainability Index](https://radon.readthedocs.io/)

## Key Metrics

- **files_analyzed:** `10`
- **average_complexity:** `{'grade': 'A', 'score': 4.0181818181818185}`
- **complexity_grade:** `A`
- **complexity_score:** `4.0181818181818185`
- **mi_output:** `E:\fenta\Downloads\The Anticloud\TIER_5_WORLD_NEURO_EMBODIED\L_BEHAVIOR1K\UPSTREAM\bddl3\setup.py - A (100.00)
E:\fenta\`

## Raw Output (first 50 lines)
```
E:\fenta\Downloads\The Anticloud\TIER_5_WORLD_NEURO_EMBODIED\L_BEHAVIOR1K\UPSTREAM\docs\gen_2026_task_data.py
    F 77:0 main - B (9)
    F 61:0 load_scene_models - B (6)
    F 50:0 load_b100_order - A (3)
    F 42:0 title_case - A (1)
E:\fenta\Downloads\The Anticloud\TIER_5_WORLD_NEURO_EMBODIED\L_BEHAVIOR1K\UPSTREAM\docs\gen_leaderboard.py
    F 90:0 generate_combined_leaderboard - B (7)
    F 28:0 load_submissions - B (6)
E:\fenta\Downloads\The Anticloud\TIER_5_WORLD_NEURO_EMBODIED\L_BEHAVIOR1K\UPSTREAM\docs\gen_task_pages.py
    F 605:0 generate_gallery - C (11)
E:\fenta\Downloads\The Anticloud\TIER_5_WORLD_NEURO_EMBODIED\L_BEHAVIOR1K\UPSTREAM\eval-jobqueue\check_results.py
    F 81:0 check_jobs - C (15)
    F 63:0 load_task_instances - B (10)
    F 163:0 main - A (3)
    F 22:0 parse_args - A (1)
E:\fenta\Downloads\The Anticloud\TIER_5_WORLD_NEURO_EMBODIED\L_BEHAVIOR1K\UPSTREAM\eval-jobqueue\generate_jobs.py
    F 196:0 build_jobs - C (15)
    F 66:0 load_task_instances - B (10)
    F 84:0 create_pseudo_resource_groups - B (10)
    F 156:0 find_compatible_pseudo_group - B (10)
    F 290:0 main - B (6)
    F 25:0 parse_args - A (1)
E:\fenta\Downloads\The Anticloud\TIER_5_WORLD_NEURO_EMBODIED\L_BEHAVIOR1K\UPSTREAM\eval-jobqueue\jobqueue.py
    F 309:0 reclaim_stale_jobs - B (7)
    M 101:4 ResourcePool.acquire - A (5)
    F 194:0 load_jobs - A (4)
    F 231:0 select_next_job - A (4)
    F 285:0 heartbeat_all_jobs_for_worker - A (4)
    F 405:0 acquire_resource - A (4)
    C
```

---
_Anticloud Independent Benchmark — 2026-09-30T17:14:20.030944+00:00_