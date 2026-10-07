# Destination benchmark results (held-out seeds 100–109, v2)

Copied from `query-data-predictor/artifacts/destination-v2/`, which also holds
the raw per-session predictions (`predictions.json`, `sessions/`) and the
generated tables (`tables/`). Those are omitted here for size and are
regenerable from seeds. See `query-data-predictor/VISION_EXPERIMENTS.md` for
the protocol and the reproduction command. The v1 results (no shared-context
pair, single earliness threshold) remain in `artifacts/destination/`.

Used by `main.tex`: `paper_table.tex` (Table 3), `paper_baselines.tex`
(Table 4), `paper_switch.pdf` (Figure 2), `paper_table_max_ci.txt` (Table 3
caption). Full results: `final_precision_table.tex`, `earliness_table.tex`,
`recovery_curves.pdf/png`, `curves.csv`, `earliness.csv`,
`earliness_per_seed.csv`, `paired_differences.csv`, `per_seed.csv`,
`manifest.json`.

`sdss/summary.json`: SkyServer log characterisation used in Section 3
(`query-data-predictor/tools/sdss_characterise.py`).

Note: 14 sessions of seed 101 first exceeded the per-session wall-clock budget
because the machine slept during the run; they were deleted and re-run, and
the final manifest records 0 failures.
