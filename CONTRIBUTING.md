# Contributing

## Workflow
- Branch names: `<topic>-<short-description>`, e.g. `transactions-contention`.
- Never commit directly to `main`. Open a PR and get at least one review.
- Commit under your own name. Make small, frequent commits.
- Never commit secrets, credentials, or large data dumps (use `.env`, which is git-ignored).

## Results CSV schema

All experiments write results to `results/<experiment>/` (e.g. `results/scalability/`) as CSV with exactly these columns:

| Column | Description |
|---|---|
| `experiment` | Experiment name: `scalability`, `replication`, `transactions`, `failure` |
| `run_id` | Unique ID per run (e.g. `scal-20250101-01`) |
| `timestamp` | ISO 8601 UTC time of the measurement |
| `nodes` | Cluster size (3, 5, 7) |
| `workload` | Workload name/params (e.g. `kv --read-percent=95`) |
| `metric` | What was measured (e.g. `p99_latency`, `qps`, `recovery_time`) |
| `value` | Numeric value |
| `unit` | Unit of `value` (e.g. `ms`, `ops/s`, `s`) |
| `notes` | Free text (optional; may be empty) |

Header row required, one metric per row (long format). Keep files small.
