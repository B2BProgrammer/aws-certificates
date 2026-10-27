------------------ AWS Certified Machine Learning Engineer - Associate Course
MLA-C0





Table of Contents
1. Data Engineering Fundamentals 
2. Storage 
3. Database 
4. Migration and Transfer 
5. Compute 
6. Containers 
7. Analytics 
8. Application Integration 
9. Security, Identity, and Compliance 
10. Networking and Content Delivery 
11. Management and Governance 
12. Machine Learning 
13. Developer Tools 
14. Everything Else 
15.  Exam Tips



--- AWS Certified Data
Engineer
Associate Course
DEA
-C01


ANALYTICS

APP INTEGRATION


CLOUD FINANCIAL
MANAGEMENT


COMPUTE

CONTAINERS

DATABASE

DEVELOPER TOOLS

FRONTEND WEB


MANAGEMENT AND GOVERNANCE


MIGRATION AND TRANSFER

NETWORKING AND CONTENT DELIVERY

SECURITY, IDENTITY, AND COMPLIANCE


STORAGE


---------------------------------------1. Data Engineering Fundamentals

    Types of Data
    Structured Data
    Unstructured Data
    Semi-Structured Data
    Properties of Data
        Volume
        Velocity
        Variety

    Data Warehouses vs. Data Lakes
        Data Warehouse 
        Data Warehouse example
        Data Lake
        Comparing the two
        Choosing a Warehouse vs. a Lake 
        Data Lakehouse
        Data Mesh

        ETL Pipelines
        ETL Pipelines: Transform
        ETL Pipelines: Load
        Managing ETL Pipelines
        Data Sources
        Common Data Formats
            CSV (Comma-Separated Values)
            JSON (JavaScript Object Notation)
            Avro
            Parquet
            A Very (intentionally) Incomplete Overview of Data Modeling
            Data Lineage
            Schema Evolution
            Database Performance Optimization
        
        Data Sampling Techniques
            Random Sampling
            Stratified Sampling
            Systemic Sampling
            Data Skew Mechanisms
            Addressing Data Skew
            Data Validation and Profiling

        SQL Review
            Aggregation
            Aggregate with CASE
            Grouping
            Nested grouping, sorting
            Pivoting
            INNER JOIN
            LEFT OUTER JOIN
            RIGHT OUTER JOIN
            FULL OUTER JOIN
            CROSS OUTER JOIN
            SQL Regular Expressions
        
        Git review
            Common git commands
            Branching with git
            Remote repositories
            Undoing changes
            Advanced git
            Git collaboration and inspection
            Git maintenance and data recovery

    
----------------------------------------------  2. Storage
        (Storing, accessing, and backing up data in AWS)

        Amazon S3 Section
            Section introduction
            Amazon S3 Use cases
            Amazon S3 - Buckets
            Amazon S3 - Objects
            Amazon S3 – Security
            S3 Bucket Policies

            Example: Public Access - Use Bucket Policy
            Example: User Access to S3 – IAM permissions
            Example: EC2 instance access - Use IAM Roles
            Advanced: Cross-Account Access – Use Bucket Policy

            Bucket settings for Block Public Access
            Amazon S3 - Versioning
            Amazon S3 – Replication (CRR & SRR)
            Amazon S3 – Replication (Notes)
            Amazon S3 – Replication Time Control (RTC)
            S3 Storage Classes
            S3 Durability and Availability
            S3 Standard – General Purpose
            S3 Storage Classes – Infrequent Access
            Amazon S3 Glacier Storage Classes
            S3 Intelligent-Tiering
            S3 Storage Classes Comparison
            S3 Storage Classes – Price Comparison Example: us-east-1
            S3 Express One Zone
            Amazon S3 – Moving between Storage Classes
            Amazon S3 – Lifecycle Rules
            Amazon S3 – Lifecycle Rules (Scenario 1)
            Amazon S3 – Lifecycle Rules (Scenario 2)
            Amazon S3 Analytics – Storage Class Analysis
            
            S3 Event Notifications
                S3 Event Notifications – IAM Permissions
                S3 Event Notifications with Amazon EventBridge
            
            S3 – Baseline Performance
                S3 Performance
                S3 Performance – S3 Byte-Range Fetches
            
            Amazon S3 – Object Encryption
            Amazon S3 Encryption – SSE-S3
            Amazon S3 Encryption – SSE-KMS
                SSE-KMS Limitation
            Amazon S3 Encryption – DSSE-KMS
            Amazon S3 Encryption – SSE-C
            Amazon S3 Encryption – Client-Side Encryption
            Amazon S3 – Encryption in transit (SSL/TLS)
            Amazon S3 – Force Encryption in Transit aws:SecureTransport
            Amazon S3 – Default Encryption vs. Bucket Policies

            S3 – Access Points
                S3 – Access Points – VPC Origin
            S3 Tables
                Wait,what’s Iceberg?
                Iceberg means S3 Tables is compatible with a lot of stuff
                Features of S3 Tables
            Table Buckets
            S3 Tables Intelligent-Tiering
            S3 Tables Replication
            S3 Tables Security

            S3 – Storage Lens
                Storage Lens – Default Dashboard
                Storage Lens – Metrics
                Storage Lens – Free vs. Paid


--------------------------------------------------------- 3. EC2 Instance Storage Section

        What’s an EBS Volume?
        EBS Volume
        EBS Volume - Example
        EBS – Delete on Termination attribute
        Amazon EBS Elastic Volumes
        Amazon EFS – Elastic File System
            EFS – Performance & Storage Classes
            EFS – Storage Classes
            EBS vs EFS – Elastic Block Storage
            EBS vs EFS – Elastic File System
        AWS Backup
            AWS Backup Vault Lock

--------------------------------------------------------- 4. Database
(Managing and querying structured and semi -structured data)

    Amazon DynamoDB (NoSQL Serverless Database)
        Traditional Architecture
        NoSQL databases
        Amazon DynamoDB
        DynamoDB - Basics
        DynamoDB – Primary Keys
        DynamoDB – Partition Keys (Exercise)
        DynamoDB in Big Data
        DynamoDB – Read/Write Capacity Modes
        R/W Capacity Modes – Provisioned
        DynamoDB – Write Capacity Units (WCU)
        Strongly Consistent Read vs. Eventually Consistent Read
        DynamoDB – Read Capacity Units (RCU)
        DynamoDB – Partitions Internal
        DynamoDB – Throttling
        R/W Capacity Modes – On-Demand
        DynamoDB – Writing Data
        DynamoDB – Reading Data
        DynamoDB – Reading Data (Query)
        DynamoDB – Reading Data (Scan)
        DynamoDB – Deleting Data
        DynamoDB – Batch Operations
        DynamoDB – PartiQL
        DynamoDB – Local Secondary Index (LSI)
        DynamoDB – Global Secondary Index (GSI)
        DynamoDB – Indexes and Throttling
        DynamoDB - PartiQL
        DynamoDB Accelerator (DAX)
        DynamoDB Accelerator (DAX) vs. ElastiCache
        DynamoDB Streams
        DynamoDB Streams & AWS Lambda
        DynamoDB – Time To Live (TTL)
        DynamoDB – Large Objects Pattern
        DynamoDB – Indexing S3 Objects Metadata
        DynamoDB – Security & Other Features
        DynamoDB – Users Interact with DynamoDB Directly
        DynamoDB – Fine-Grained Access Control


     -- Amazon RDS (Relational Database Service)
        What is RDS?
        ACID
        Amazon Aurora
            Aurora Security
            Using the LOCK command
            Examples (MySQL)
        Amazon RDS best practices
        Amazon RDS operational guidelines
        Query optimization in RDS
        DB-specific tweaks
        Amazon Aurora
            Aurora High Availability and Read Scaling
            Aurora DB Cluster
            Features of Aurora
            Amazon Aurora as a Vector Store
        
        DocumentDB
        Amazon MemoryDB for Redis
        Amazon Keyspaces (for Apache Cassandra)
        Amazon Neptune
            Amazon Neptune – Query Languges
        Amazon Timestream
            Amazon Timestream – Architecture

    --Amazon Redshift (Fully -managed, petabyte -scale data warehouse)
        What is Redshift?
            Redshift Use -Cases
            Redshift architecture
            Redshift Spectrum
            Redshift Performance
            Redshift Durability
            Scaling Redshift
            Redshift Distribution Styles
            EVEN distribution
            KEY distribution
            ALL distribution
            Importing / Exporting data
            COPY command: More depth
            Redshift copy grants for cross-region snapshot copies
            DBLINK
            Integration with other services
            Redshift Workload Management (WLM)
            Concurrency Scaling
            Automatic Workload Management
            Manual Workload Management
            Short Query Acceleration (SQA)
            Resizing Redshift Clusters
            VACUUM command
            Newer Redshift features

        -- Amazon Redshift ML
            Redshift anti -patterns
            Redshift security concerns
            Redshift Serverless
                Redshift Serverless: Getting Started
                Resource Scaling in Redshift Serverless
                Redshift Serverless 
                Redshift Serverless: Monitoring
                Redshift Materialized Views
                Using Materialized Views
                Redshift Data Sharing
                Redshift Lambda UDF
                Redshift Federated Queries
                Redshift System Tables and Views
                Redshift Data API
                    Redshift Data API: Other use cases
                    Redshift Data API: Finer Points

--------------------------------------------4. Migration and Transfer (Moving data into AWS)

            AWS Application Discovery Service
            AWS Application Migration Service (MGN)
            DMS – Database Migration Service
            DMS Sources and Targets
            AWS Schema Conversion Tool (SCT)
            DMS - Continuous Replication
            AWS DMS – Multi-AZ Deployment
            AWS DataSync
                AWS DataSync NFS / SMB to AWS (S3, EFS, FSx…
                AWS DataSync Transfer between AWS storage services
                AWS Snowball
                Data Migrations with Snowball
            Diagrams
            What is Edge Computing?
            AWS Data Exchange
                AWS Data Exchange  – Other Products
            AWS Transfer Family

------------------------------------ 5. Compute
Transforming Data in AWS


            EC2 in Big Data
            AWS Graviton

            AWS Lambda - Serverless data processing
                What is Lambda?
                    Example: Serverless Website
                    Example: Order history app
                    Example: Transaction rate alarm
                Why not just run a server?
                Main uses of Lambda
                Supported languages
                Lambda triggers
                Lambda and Amazon Opensearch Service
                Lambda and Redshift
                Lambda + Kinesis
                Cost Model
                Other promises
                Anti-patterns
                Lambda – File Systems Mounting
                Lambda – Storage Options

                AWS SAM
                    AWS SAM – Recipe
                    Deep Dive into SAM Deployment
                    SAM Accelerate (sam sync)
                    SAM Accelerate (sam sync) – Examples
                AWS Batch
                    AWS Batch vs Glue
                

--------------------------------------------------6. Containers
Packaging applications in AWS

            Containers on AWS
                What is Docker?
            Docker on an OS
                Where are Docker images stored?
                Docker vs. Virtual Machines
                Getting Started with Docker
                Docker Containers Management on AWS
                Amazon ECS - EC2 Launch Type
                Amazon ECS – Fargate Launch Type
                Amazon ECS – IAM Roles for ECS
                Amazon ECS – Load Balancer Integrations
                Amazon ECS – Data Volumes (EFS)
                Amazon ECS – Data Volumes (S3 Files)
                
                Amazon ECR
                Amazon EKS Overview
                    Amazon EKS - Diagram
                    Amazon EKS – Node Types
                    Amazon EKS – Data Volumes

--------------------------- 7. Analytics
Extracting structure and meaning from data in AWS    

                - AWS Glue (Table definitions and ETL)
                    What is Glue?
                    Glue Crawler / Data Catalog
                    Glue and S3 Partitions
                    Glue + Hive
                    Glue ETL
                        Glue ETL: The DynamicFrame
                        Glue ETL - Transformations
                        Glue ETL: ResolveChoice
                        Glue ETL: Modifying the Data Catalog
                    AWS Glue Development Endpoints
                        Running Glue jobs
                        Glue cost model
                        Glue Anti -patterns
                        No longer an anti-pattern: streaming
                        AWS Glue Studio
                        AWS Glue Data Quality
                        More on Data Quality Definition Language (DQDL)
                        AWS Glue Data Quality
                        AWS Glue DataBrew
                        Handling (PII) in DataBrew Transformations
                        Glue Workflows
                        Glue Workflow Triggers
                        Glue Flex Jobs
                        
                    AWS Lake Formation
                        AWS Lake Formation: Pricing
                        AWS Lake Formation: Building a Data Lake
                        AWS Lake Formation: The Finer Points
                        Data Permissions in Lake Formation
                        Data Filters in Lake Formation

                    Amazon Athena - Serverless interactive queries of S3 data
                        What is Athena? 
                        Some examples
                        Athena + Glue
                        Athena Workgroups
                        Athena cost model
                        Athena Security
                        Athena anti-patterns
                        Athena: Optimizing performance
                        Athena ACID transactions
                        Athena Fine-Grained Access to AWS Glue Data Catalog
                        Wait,what’s Iceberg?
                        Iceberg + AWS Glue / S3
                        Migrating Glue Data Catalogs to Iceberg
                        CREATE TABLE AS SELECT
                        Athena Federated Queries
                        Apache Spark
                        How Spark Works
                        Spark Components
                            Spark Structured Streaming A constantly growing DataSet
                            Spark Streaming + Kinesis
                            Spark + Redshift
                            Amazon Athena for Apache Spark

            EMR - Elastic MapReduce                            
                What is EMR?
                An EMR Cluster
                EMR Usage
                EMR / AWS Integration
                EMR Storage
                EMR promises
                EMR Managed Scaling
                EMR Serverless
                Using EMR Serverless
                EMR Serverless Application Lifecycle
                Pre-Initialized Capacity
                EMR Serverless Security 
                EMR on EKS

                Kinesis Data Streams
                    Kinesis Data Streams – Capacity Modes
                    Kinesis Data Streams Security

                    Kinesis Producers
                    Kinesis Producer SDK - PutRecord(s)
                    AWS Kinesis API – Exceptions
                    Kinesis Producer Library (KPL)
                    Kinesis Producer Library (KPL) Batching
                    Kinesis Producer Library – When not to use
                    Kinesis Agent

                    Kinesis Consumers - Classic
                        Kinesis Consumer SDK - GetRecords
                        Kinesis Client Library (KCL)
                        Kinesis Connector Library
                        AWS Lambda sourcing from Kinesis
                       
                    Kinesis Enhanced Fan Out
                    Enhanced Fan-Out vs Standard Consumers
                    Kinesis Operations – Adding Shards
                    Kinesis Operations – Merging Shards
                    
                    Out-of-order records after resharding
                    Kinesis Operations – Auto Scaling
                    Kinesis Scaling Limitations
                    Kinesis Data Streams – Handling Duplicates For Producers
                    Kinesis Data Streams – Handling Duplicates For Consumers
                    Kinesis Security
                    
                    Kinesis Data Firehose

                        AWS Kinesis Data Firehose
                        Kinesis Data Firehose Delivery Diagram
                        Firehose Buffer 
                        Kinesis Data Streams vs Firehose
                        Troubleshooting Kinesis Data Stream Producers: Performance
                        Other Kinesis Data Stream Producer Issues

                        Troubleshooting Kinesis Data Stream Consumers

                
                -- Kinesis Data Analytics /Managed Service for Apache Flink
Querying streams of data

            Amazon Kinesis Data Analytics for SQL Applications
                Reference tables are cool
                Kinesis Data Analytics + Lambda
                Managed Service for Apache Flink
                Apache Flink Capabilities
                Common use-cases
                Kinesis Analytics
                    RANDOM_CUT_FOREST
                    Amazon Managed Streaming for Apache Kafka (Amazon MSK)
                    Apache Kafka at a high level
                    MSK – Configurations
                    MSK – Security
                    MSK – Monitoring
                    MSK Connect
                    MSK Serverless
                    Kinesis Data Streams vs Amazon MSK


        -- Amazon Opensearch Service (formerly Elasticsearch) 
            Petabyte-scale analysis and reporting

            What is Opensearch ?
            What are Dashboards
            Opensearch applications
            Opensearch concepts
            An index is split into shards
            Redundancy
            Amazon OpenSearch Service (Managed)
            Amazon Opensearch options
                Cold / warm / ultrawarm / hot storage
                Index State Management
                More Index Management
                Cross-cluster replication
                Opensearch Stability
                Amazon Opensearch Security
                Securing Dashboards
                Amazon Opensearch anti-patterns
                Amazon Opensearch performance
                Amazon OpenSearch Serverless

        --- Amazon Quick Suite (formerly QuickSight)
            Business analytics and visualizations in the cloud


            What is Quick Suite / Quick Sight?
            Quick Sight Data Sources
            SPICE
            Quick Sight Use Cases
            Quick Sight Anti-Patterns
            Quick Sight Security
            Quick Sight + Redshift: Security
            Quick Sight / Redshift / RDS cross-region
            Quick Sight / Redshift / RDS crossaccount
            Quick Sight User Management
            Quick Sight pricing
            Quick Sight Dashboards
            Quick Sight Machine Learning Insights
            Quick Sight Calculated Fields
            Level -Aware Calculations (LAC)
            Level-Aware Calculations – Window (LAC-W)
            FLOAT vs FIXED Data Types


        ---- Application Integration
                Moving data between systems in AWS

            AWS SQS What’s a queue?
            AWS SQS – Standard Queue
            SQS – Producing Messages
            SQS – Consuming Messages
            AWS SQS – FIFO Queue
            SQS Extended Client
            AWS SQS Use Cases
            SQS Limits
            AWS SQS Security

            Kinesis Data Stream vs SQS
            SQS vs Kinesis – Use cases
            Amazon SQS – Dead Letter Queue (DLQ)
            SQS DLQ – Redrive to Source
            
            Amazon SNS
            SNS integrates with a lot of AWS services
            Amazon SNS – How to publish
            Amazon SNS – Security
            SNS + SQS: Fan Out
            Application: S3 Events to multiple queues
            Application: SNS to Amazon S3 through Kinesis Data Firehose
            Amazon SNS – FIFO Topic
            SNS FIFO + SQS FIFO: Fan Out
            SNS – Message Filtering

            AWS Step Functions
                Step Functions – Examples Train a Machine Learning Model
                Step Functions – Examples Tune a Machine Learning Model
                Step Functions – Examples Manage a Batch Job

            AWS Step Functions
            Amazon AppFlow
            Amazon EventBridge (formerly CloudWatch Events)
                Amazon EventBridge Rules
                Amazon EventBridge
                Amazon EventBridge – Schema Registry
                Amazon EventBridge – Resource-based Policy
            Amazon Managed Workflows for Apache Airflow (MWAA)
            Sample DAG in Airflow
            Airflow + MWAA
                Amazon MWAA Integration
                Amazon MWAA Architecture

---------------- 9. Security, Identity, and Compliance
                    Securing data in AWS 
                    
            Principle of Least Privilege
            Data Masking and Anonymization
            Key Salting
                Key Salting: Example
                Keeping Data Where it Belongs
                IAM: Users & Groups
                IAM: Permissions
                IAM Policies inheritance
                IAM Policies Structure
                IAM – Password Policy
                Multi Factor Authentication - MFA
                MFA devices options in AWS
                IAM Roles for Services

                Why encryption? Encryption in flight (TLS / SSL)
                Why encryption? Server-side encryption at rest

                Why encryption? Client-side encryption
            
            AWS KMS (Key Management Service)
                KMS Keys Types
                AWS KMS (Key Management Service)            
                Copying Snapshots across regions
                KMS Key Policies
                Copying Snapshots across accounts

            AWS Macie
            AWS Secrets Manager
                AWS Secrets Manager – Multi-Region Secrets
            AWS WAF – Web Application Firewall
                WAF – Fixed IP while using WAF with a Load Balancer
            AWS Shield: protect from DDoS attack
            Security - Kinesis
            Security - SQS
            Security – AWS IoT
            Security – Amazon S3
            Security – DynamoDB
            Security - RDS
            Security - Aurora
            Security - Lambda
            Security - Glue
            Security - EMR
            Security – EMR Encryption (security config)
            Security – OpenSearch Service
            Security - Redshift
            Security - Athena
            Security - Quicksight


---------------- 10. Networking and Content Delivery
Connecting the pipes in AWS


            VPC & Subnets Primer
            VPC Diagram
            Internet Gateway & NAT Gateways
            Network ACL & Security Groups
            Network ACLs vs Security Groups
            VPC Flow Logs
            VPC Peering
            VPC Endpoints
            Site to Site VPN & Direct Connect
            VPC Closing Comments
            AWS PrivateLink (VPC Endpoint Services)

            What is DNS?
            How DNS Works

            Amazon Route 53
                Route 53 – Records
                Route 53 – Record Types
                Route 53 – Hosted Zones
                Route 53 – Public vs. Private Hosted Zones
            Amazon CloudFront
                CloudFront – Origins
                CloudFront at a high level
                CloudFront – S3 as an Origin
                CloudFront vs S3 Cross Region Replication
                CloudFront – ALB or EC2 as an origin Using VPC Origins
                CloudFront – ALB or EC2 as an origin Using Public Network
                CloudFront – Cache Invalidations

--------------------------- 11. Management and Governance
            Monitoring the big picture in AWS


            Amazon CloudWatch Metrics
            CloudWatch Metric Streams
            CloudWatch Logs
                    CloudWatch Logs - Sources
                    CloudWatch Logs Insights
                    CloudWatch Logs – S3 Export
                    CloudWatch Logs Subscriptions
                    CloudWatch Logs Aggregation Multi-Account & Multi Region
                    CloudWatch Logs Subscriptions
                    CloudWatch Logs for EC2
                    CloudWatch Logs Agent & Unified Agent
            CloudWatch Unified Agent – Metrics
            CloudWatch Alarms
            CloudWatch Alarm Targets
            CloudWatch Alarms – Composite Alarms
            EC2 Instance Recovery
            CloudWatch Alarm: good to know

            AWS CloudTrail
                CloudTrail Diagram
            
            CloudTrail Events
            CloudTrail Insights
            CloudTrail Events Retention
            AWS CloudTrail Lake
                Example of an advanced event selector
                Querying CloudTrail Lake
            AWS Config
            Config Rules
            AWS Config Resource 
                Config Rules – Remediations
                Config Rules – Notifications
            CloudWatch vs CloudTrail vs Config
            For an Elastic Load Balancer

            What is CloudFormation
                Benefits of AWS CloudFormation (1/2)
                Benefits of AWS CloudFormation (2/2)
            CloudFormation + Infrastructure Composer

            SSM Parameter Store
                SSM Parameter Store Hierarchy
                Standard and advanced parameter tiers
                Parameters Policies (for advanced parameters)

            Well Architected Framework - General Guiding Principles
                Well Architected Framework 6 Pillars
                AWS Well-Architected Tool

            Amazon Managed Grafana

------------------------12. Machine Learning
            Learning from data in AWS


            Amazon SageMaker AI
            SageMaker Feature Store
            Where the features come from is up to you
            How SageMaker Feature Store Organizes Your Data
            Data Ingestion (streaming or batch)
            SageMaker Feature Store Security
            SageMaker ML Lineage Tracking
            Lineage Tracking Entities
            Querying Lineage Entities


            --SageMaker Ground Truth
             (NOTE: GROUND TRUTH IS DEPRECATED AS OF JULY 30 2026. IT REMAINS IN THE EXAM GUIDE HOWEVER)
                What is Ground Truth?
                Who are these human labelers?
                Ground Truth Plus
                Other ways to generate training labels
                Amazon Mechanical Turk
                SageMaker Canvas
                SageMaker Data Wrangler
                Data Wrangler sources
                Data Wrangler: Import Data
                Data Wrangler: Preview Data
                Data Wrangler: Visualize Data
                Data Wrangler: Transform Data
                Data Wrangler: Quick Model
                Data Wrangler: Export Data Flow
                Data Wrangler Troubleshooting
      
            Foundation Models
                AWS Foundation Models (Base Models)
                Amazon Bedrock
                The Bedrock API Endpoints
                    Bedrock IAM permissions
                
                Amazon Bedrock: Model Access
                
                Fine-tuning
                        Fine-tuning in Bedrock: “Custom Models”
                        “Continued Pre-Training”
                Low-Rank Adaptation (LoRA)

                Retrieval Augmented Generation (RAG)
                        RAG: Pros and Cons
                        RAG: Example Approach (winning at Jeopardy!)
                        Choosing a Database (Knowledge Base Data Store) for RAG
                        Embeddings
                            Embeddings are vectors, so store them in…
                        RAG Example with a Vector Database: Making Data from Star Trek, by Cheating
                        RAG in Bedrock: Knowledge Bases
                        Using Knowledge Bases
                            Let’s Make a Knowledge Base
                            Breaking up the R in RAG
                            Pre-Retrieval
                        More on Chunking
                            Chunking with Bedrock: Standard Chunking
                            Chunking with Bedrock: Hierarchical Chunking
                            Chunking with Bedrock: Semantic Chunking
                        Optimizing your Embeddings
                        Sparse vs. Dense Embeddings
                        Optimizing Retrieval with Metadata
                        Keeping Your KB Up to Date
                        OpenSearch as a Vector Store
                            OpenSearch Vector Engines
                                OpenSearch as a Vector Store: Finer Points
                            Amazon Aurora as a Vector Store 

                            Amazon Quick
                                Amazon Quick – Capabilities
                                Amazon Quick + IAM Identity Center
                                Amazon Quick – Integrations
                                Apps in Amazon Quick
                                Amazon Quick Example

                            Amazon Kendra


---------------------------------- 13. Developer Tools 
                Developing apps around your data in AWS
                
        
            How can users access AWS ?
            Example (Fake) Access Keys
            What’s the AWS CLI?
            What’s the AWS SDK?
            AWS Cloud Development Kit (CDK)
            CDK in a diagram
            CDK vs SAM
            CDK + SAM
            CDK Hands -On
            AWS CodeDeploy
            AWS CodeCommit
            AWS CodeBuild
            AWS CodePipeline


------------------------  14. Everything Else
            Cost management, front-end and mobile access      
            
            
            AWS Budgets
            Cost Explorer
                Cost Explorer – Monthly Cost by AWS Service
                Cost Explorer– Hourly & Resource Level
                Cost Explorer – Savings Plan Alternative to Reserved Instances
                Cost Explorer – Forecast Usage
                Example: Building a Serverless API
                
            AWS API Gateway
                API Gateway – Integrations High Level
                API Gateway – AWS Service Integration Kinesis Data Streams example
                API Gateway - Endpoint Types
                API Gateway – Security
                




































                        


















