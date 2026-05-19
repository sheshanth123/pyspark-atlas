# PySpark Master Topic List
> Compiled from leading books and courses on PySpark, Apache Spark, Data Engineering, and Data Science.  
> Sources: *Spark: The Definitive Guide*, *Learning Spark 2nd Ed.*, *Advanced Analytics with PySpark*, *High Performance Spark*, *Data Analysis with Python and PySpark*, *Learning PySpark* — and courses from DataCamp, Udemy, and Codecademy.

---

## Bucket 1 — Big Data Fundamentals & Spark Foundations

### What is Big Data
- 3 Vs: volume, velocity, variety
- Big data ecosystem overview
- Challenges of large-scale data processing

### Apache Spark Overview
- History and philosophy of Spark
- Spark vs Hadoop MapReduce
- Spark vs pandas / Dask
- Present and future of Spark

### Spark Architecture
- Driver and executors
- Cluster manager
- DAG execution model
- Lazy evaluation
- Transformations vs actions
- Spark UI
- SparkSession
- RDD vs DataFrame vs Dataset

### Spark Language APIs
- Python (PySpark)
- Scala
- Java
- R (SparkR / sparklyr)

### PySpark Setup & Environment
- Installing PySpark (pip / conda)
- Databricks Community Edition
- VirtualBox / Docker local setup
- AWS EC2 for Spark
- Google Cloud Platform (GCP) / Dataproc
- Azure Databricks setup
- Jupyter Notebooks with PySpark
- SparkContext and SparkSession initialisation

---

## Bucket 2 — DataFrames & Spark SQL

### DataFrames Basics
- Creating DataFrames
- Schemas and data types
- Columns and rows
- Partitions
- Spark types overview

### DataFrame API Operations
- select, selectExpr
- filter / where
- groupBy / agg
- orderBy / sort
- Join operations
- union / concat
- withColumn / rename columns
- drop columns
- distinct / unique rows
- Random sampling and splits
- collect / show

### Built-in Functions
- Math and numeric functions
- String functions and regex
- Date and timestamp functions
- Boolean operations
- Working with nulls (coalesce, fillna, dropna)
- Complex types: arrays, maps, structs
- explode
- User-defined functions (UDFs)
- Pandas UDFs

### Aggregations
- count, countDistinct, sum, avg, min, max
- groupBy aggregations
- Window functions
- Ranking functions (rank, dense_rank, row_number)
- Cumulative aggregations
- Pivot tables

### Joins
- Inner join
- Left / right / full outer join
- Cross join
- Broadcast joins
- Join strategies and shuffle
- Complex join conditions

### Spark SQL
- SQL interface (spark.sql)
- SparkSQL Thrift JDBC/ODBC server
- Spark metastore and catalogs
- Creating tables and views
- Managed vs external tables
- Caching tables
- Subqueries
- CASE WHEN statements
- Complex types in SQL
- Hive integration
- Delta tables and SQL

---

## Bucket 3 — Data Sources, Sinks & File Formats

### Reading and Writing Data
- CSV
- JSON
- Parquet
- ORC
- Avro
- Delta Lake format
- Text files

### Data Source Connectors
- HDFS
- Amazon S3
- Azure Data Lake (ADLS)
- Google Cloud Storage (GCS)
- JDBC (relational databases)
- HBase / Cassandra
- MongoDB

### Schema Inference and Management
- inferSchema
- Explicit schema definition (StructType)
- Schema evolution
- Schema validation

### Partitioning and Storage Optimisation
- partitionBy on write
- repartition vs coalesce
- Bucketing
- File compaction

---

## Bucket 4 — Data Engineering Pipelines & ETL

### ETL / ELT Pipeline Design
- Batch processing
- Incremental loading
- Idempotent pipelines
- Pipeline orchestration patterns
- File format converters
- Files-to-database loaders

### Delta Lake
- ACID transactions
- Time travel / versioning
- Delta table updates and deletes
- MERGE (upsert)
- Schema enforcement and evolution
- Incremental loads with Delta
- OPTIMIZE and Z-order
- VACUUM

### Workflow Orchestration
- Apache Airflow DAGs
- Databricks workflows and jobs
- Job scheduling and triggers
- Cron scheduling
- Monitoring with Spark UI
- CI/CD pipelines for Spark

### Data Quality and Cleaning
- Handling missing / null values
- Data validation
- Deduplication
- Type casting and coercion
- Outlier detection
- Standardising formats

### Cloud Integrations
- Azure Data Factory pipelines
- AWS Glue and EMR
- GCP Dataproc
- Authentication (access keys, SAS tokens, service principals)
- Azure Key Vault / Databricks secret scopes
- Unity Catalog data governance

### Kafka Integration
- Reading from Kafka
- Writing to Kafka
- Kafka + Spark Streaming patterns

---

## Bucket 5 — Structured Streaming & Real-Time Processing

### Structured Streaming Basics
- Streaming vs batch
- Micro-batch processing
- Trigger intervals
- Watermarks
- Output modes (append, complete, update)

### Streaming Sources and Sinks
- Kafka source / sink
- File source (CSV, JSON, Parquet)
- Socket source
- Delta Lake sink
- HDFS / cloud storage sink

### Stateful Streaming Operations
- Windowing (tumbling, sliding, session)
- Aggregations on streams
- Stream–stream joins
- Stream–table joins
- Late data handling

### Stream Processing in Lakehouse
- Streaming to Delta Lake
- Continuous processing
- Fault tolerance and checkpointing
- End-to-end exactly-once semantics

---

## Bucket 6 — Machine Learning with PySpark (MLlib)

### MLlib Overview
- ML pipelines API
- Transformers
- Estimators
- Pipeline stages
- CrossValidator
- ParamGridBuilder

### Feature Engineering
- VectorAssembler
- StringIndexer
- OneHotEncoder
- Bucketizer
- StandardScaler / normaliser
- PCA
- Polynomial expansion
- Feature selection (ChiSqSelector)
- TF-IDF
- Word2Vec
- Tokenisation
- Stop words removal
- N-grams

### Supervised Learning — Regression
- Linear regression
- Logistic regression
- Decision trees
- Random forests
- Gradient boosted trees (GBT)
- Model evaluation (RMSE, MAE, R²)
- Hyperparameter tuning

### Supervised Learning — Classification
- Logistic regression classification
- Decision tree classifier
- Random forest classifier
- Naive Bayes
- Model evaluation (accuracy, AUC, F1)
- Cross-validation

### Unsupervised Learning
- K-means clustering
- Choosing K (elbow method)
- Latent Dirichlet Allocation (LDA)
- Topic modelling
- Curse of dimensionality
- Anomaly / outlier detection

### Recommendation Systems
- Collaborative filtering
- Alternating Least Squares (ALS)
- Computing AUC for recommendations
- Hyperparameter selection
- MovieLens dataset examples
- Million Songs dataset

### Deep Learning with Spark
- Integrating PyTorch with PySpark
- Distributed deep learning
- Image embeddings and similarity search

---

## Bucket 7 — Advanced Analytics & Data Science Patterns

### NLP at Scale
- Spark NLP library
- Text parsing and tokenisation
- TF-IDF at scale
- LDA topic modelling
- Sentiment analysis
- Text classification

### Geospatial Analysis
- GeoJSON basics
- GeoPandas integration
- Sessionisation in PySpark
- Secondary sorts

### Time Series Analysis
- Converting datetime strings
- Handling invalid timestamps
- Sessionisation
- Time-based aggregations
- Window-based feature engineering

### Graph Analytics
- GraphX overview
- Graph algorithms (PageRank, connected components)
- Neo4j integration

### Financial / Risk Analytics
- Value at Risk (VaR) methods
- Monte Carlo simulation
- Multivariate normal distribution
- Factor weight determination

### Genomics / Scientific Computing
- ADAM genomics framework
- Analysing genomics data at scale
- Predicting transcription factor binding sites

---

## Bucket 8 — Performance Tuning & Optimisation

### Spark Execution Model
- DAG and stages
- Tasks and slots
- Shuffle operations
- Spill to disk
- Catalyst optimizer
- Tungsten execution engine

### Performance Tuning Techniques
- Partition tuning (repartition / coalesce)
- Caching and persistence (cache, persist)
- Broadcast joins for small tables
- Avoiding data skew
- Predicate pushdown
- Columnar storage benefits (Parquet / ORC)

### Memory and Resource Management
- Executor memory configuration
- Driver memory
- Memory fractions (storage vs execution)
- Garbage collection tuning
- Off-heap memory

### Explain Plans and Debugging
- Reading explain plans (logical, physical)
- Spark UI analysis (jobs, stages, tasks)
- Identifying bottlenecks
- Debugging PySpark jobs
- Unit testing Spark code

### Cluster Management
- Local mode
- Standalone mode
- YARN
- Mesos
- Kubernetes
- Cluster configurations and policies
- Cost control strategies

---

## Bucket 9 — SQL for Data Engineering

### SQL Fundamentals
- SELECT, WHERE, GROUP BY, ORDER BY
- HAVING clause
- LIMIT and OFFSET
- Aliases

### Advanced SQL
- Window functions (OVER, PARTITION BY)
- Ranking (RANK, DENSE_RANK, ROW_NUMBER, NTILE)
- Cumulative totals
- Complex joins (self, cross, lateral)
- Subqueries and CTEs
- CASE WHEN
- UNION / INTERSECT / EXCEPT

### Database and Data Warehouse Concepts
- Relational database fundamentals
- Data warehouse vs data lake vs lakehouse
- Dimensional modelling (star schema, snowflake)
- Indexing strategies
- Query optimisation

### Data Stores
- PostgreSQL setup and use
- Hive
- HBase
- NoSQL databases
- HDFS basics

---

## Bucket 10 — Python for Data Engineering

### Python Essentials
- Basic data types and control flow
- Functions and modules
- List / dict / set comprehensions
- Error handling (try/except)
- File I/O

### Python Collections and OOP
- Lists, tuples, dictionaries, sets
- Iterators and generators
- Classes and objects
- Decorators

### Data Processing with Python
- pandas DataFrames
- pandas vs PySpark comparison
- NumPy
- Reading / writing CSV, JSON, Parquet with pandas
- Database programming (psycopg2, SQLAlchemy)

### Software Engineering for Data Engineering
- Project structure (scripts/, configs/)
- Virtual environments
- Unit testing (pytest)
- Git branching and merging
- CI/CD basics
- Modular reusable code
- Version control workflows

---

## Bucket 11 — Cloud Platforms & DevOps

### Databricks
- Databricks architecture
- Cluster types and configurations
- Notebooks and magic commands
- Databricks utilities (dbutils)
- Databricks workflows
- Unity Catalog
- Delta Live Tables

### AWS for Big Data
- S3 as data lake
- EMR (Elastic MapReduce)
- EC2 for Spark
- Glue ETL service
- Kinesis (streaming)
- IAM roles and policies

### Azure
- Azure Data Lake Storage (ADLS)
- Azure Data Factory (ADF)
- Azure Databricks
- Azure Key Vault secrets
- Power BI integration

### Google Cloud Platform
- GCS as data lake
- Dataproc (managed Spark)
- BigQuery integration
- Cloud Shell and billing

### Infrastructure Tooling
- Docker for Spark environments
- Containerised pipeline deployment
- Environment management (dev vs prod)
- Ticket-based deployments

---

## Summary

| # | Bucket | Topics | Subtopics |
|---|--------|--------|-----------|
| 1 | Big Data Fundamentals & Spark Foundations | 5 | 24 |
| 2 | DataFrames & Spark SQL | 6 | 42 |
| 3 | Data Sources, Sinks & File Formats | 4 | 19 |
| 4 | Data Engineering Pipelines & ETL | 6 | 29 |
| 5 | Structured Streaming & Real-Time Processing | 4 | 17 |
| 6 | Machine Learning with PySpark (MLlib) | 7 | 44 |
| 7 | Advanced Analytics & Data Science Patterns | 6 | 26 |
| 8 | Performance Tuning & Optimisation | 5 | 27 |
| 9 | SQL for Data Engineering | 4 | 21 |
| 10 | Python for Data Engineering | 4 | 20 |
| 11 | Cloud Platforms & DevOps | 5 | 27 |
| **Total** | | **56** | **296** |
