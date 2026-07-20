```mermaid
flowchart TD

    A[Flight Dataset] --> B[Apache Airflow]

    B --> C[S3 Bronze Layer]

    C --> D[PySpark ETL]

    D --> E[S3 Silver Parquet]

    E --> F[Gold Analytics]

    F --> G[AWS Glue Catalog]

    G --> H[Amazon Athena]

    H --> I[CloudWatch Monitoring]
```