# gcp-data-engineering-labs

Practice and lab repo for GCP Data Engineering. Training/practice code only —
a polished end-to-end project gets promoted to its own separate repo later.

Scope: **GCP only.** Azure work lives in `azure-data-engineering-labs`.

## Structure

| Folder | Contents | Priority |
| --- | --- | --- |
| `00-fundamentals/` | Python, SQL, Linux, GCP basics (console/shell/SDK, regions/zones, IAM, resource hierarchy) | Base |
| `01-gcs/` | Buckets, lifecycle, versioning, transfer service | Medium |
| `02-cloud-sql/` | Instances, import/export, DMS migration | Low |
| `03-bigquery/` | SQL, partitioning/clustering, query plans, views, case studies | High |
| `04-dataproc/` | PySpark jobs, submission, optimization | HIGHEST |
| `05-dataflow/` | Apache Beam batch/streaming, templates | High |
| `06-pubsub/` | Topics, subscriptions, publisher/subscriber code | Medium |
| `07-composer/` | Airflow DAGs, plugins, CI/CD notes | High |
| `08-data-fusion/` | Pipeline exports, Wrangler notes | Low |
| `09-cloud-functions/` | Event-driven triggers (GCS to BigQuery) | Low |
| `10-terraform/` | IaC for GCS, Dataproc, BigQuery | Low |
| `99-project/` | End-to-end batch + streaming pipeline | Portfolio |
| `interview/` | Interview questions, architecture scenarios, mock notes | High |

## Conventions

- Code lives in Git (durable); cloud runs it (disposable).
- Never commit secrets, tokens, PATs, or service-account JSON. This is a public repo.
- No data files. Each folder carries a `README.md` placeholder because Git tracks files, not folders.
- Notebooks committed as source (`.py` / `.ipynb`).
- Composer DAGs: authored here, deployed to the environment GCS bucket.
