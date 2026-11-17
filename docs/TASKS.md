# Tasks

## Setup phase

| # | Task | Owner | Deadline |
|---|---|---|---|
| 1 | **(HIGHEST PRIORITY, blocks everyone)** Working Docker Compose setup with parameterized node count, pinned version, init script, tested `cockroach workload` commands, README | Member 1 | TBD |
| 2 | Set up local Python environment; confirm connection to the cluster with psycopg | Members 2-5 | TBD |

## Experiments and analysis

| # | Task | Owner | Deadline |
|---|---|---|---|
| 3 | SQL layer / query processing: architecture write-up and query-planning feature demo | Member 1 | TBD |
| 4 | Data pipeline: shared loading/plotting code in `analysis/`, results integration for report | Member 1 | TBD |
| 5 | Distribution layer, data storage and sharding: write-up; scalability experiment (`experiments/scalability/`) | Member 2 | TBD |
| 6 | Replication layer, replication: write-up; replication experiment (`experiments/replication/`) | Member 3 | TBD |
| 7 | Transaction layer, transaction processing: write-up; transaction behaviour experiment (`experiments/transactions/`) | Member 4 | TBD |
| 8 | Storage layer (Pebble), failure recovery: write-up; node-failure resilience experiment (`experiments/failure/`) | Member 5 | TBD |
| 9 | Results CSVs committed in `results/<experiment>/` per schema in CONTRIBUTING.md | Members 2-5 | TBD |
