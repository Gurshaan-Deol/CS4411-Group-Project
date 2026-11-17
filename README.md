# CockroachDB: Architectural Analysis and Case Study

CS4411 Databases II, Western University. An architectural analysis of CockroachDB (SQL, distribution, replication, transaction and storage layers) with a hands-on case study: multi-node Docker clusters (3/5/7 nodes) and one experiment per layer.

The written report is in Overleaf and is **not** stored in this repo.

## Team

| Member | Name | GitHub | Architecture topic / feature | Experiment |
|---|---|---|---|---|
| 1 | `<name>` | `<github-username>` | SQL layer, query processing; case study setup (Docker cluster); later: data pipeline and report integration | Setup + pipeline |
| 2 | `<name>` | `<github-username>` | Distribution layer; data storage and sharding | Scalability |
| 3 | `<name>` | `<github-username>` | Replication layer; replication | Replication |
| 4 | `<name>` | `<github-username>` | Transaction layer; transaction processing | Transaction behaviour |
| 5 | `<name>` | `<github-username>` | Storage layer (Pebble); failure recovery | Node-failure resilience |

## CockroachDB version

TODO: pin exact version (Member 1)

## Folder overview

| Folder | Purpose | Owner |
|---|---|---|
| `setup/` | Docker Compose and init scripts | Member 1 |
| `experiments/scalability/` | Scalability experiment | Member 2 |
| `experiments/replication/` | Replication experiment | Member 3 |
| `experiments/transactions/` | Transaction behaviour experiment | Member 4 |
| `experiments/failure/` | Node-failure resilience experiment | Member 5 |
| `analysis/` | Shared plotting/data code | Member 1 |
| `results/` | Small CSV outputs, one subfolder per experiment | All |
| `docs/` | Notes, diagrams, architecture write-ups, [TASKS.md](docs/TASKS.md) | All |

## Getting started

Prerequisites: Docker + Docker Compose, Python 3, git.

```bash
python -m venv .venv
# activate: .venv\Scripts\activate (Windows) | source .venv/bin/activate (macOS/Linux)
pip install -r requirements.txt
```

> **TODO (Member 1):** Add cluster start instructions here: how to start 3/5/7 nodes, run the init script, connect with the `cockroach` CLI, run `cockroach workload`, and tear down.

See [CONTRIBUTING.md](CONTRIBUTING.md) for workflow and the results CSV schema.
