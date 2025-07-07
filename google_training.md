# Google Training

## July 3, 2025

### Cloud Leader Learning Path

#### Benefits

- Setting up your on premesis computing can take months due to procurement, high costs due to physical space, power, personnel management etc.
- Scaling can also be difficult, and the process long and costly when demand increases.
- Could end up with low utilization and extra overhead(costs)

- **Private cloud** is where infrastructure is dedicated to a single org. aka single tenant or corporate cloud
- **Public** is can be multi-tenant.
- Generally when people say "cloud", it is the public cloud.
- **Hybrid** is a combo of on prem/private and public
- **Multicloud** uses multiple public providers

- Scalability
- Flexibility
    - Accessibility anywhere - no need to manually scale services

##### Why would you choose Cloud services?

- Be the best at understanding and using data
- Best infrastructure
- Best hybrid workplace
- Security
- Sustainability

### The Primary Capabilities

- Data
- Open Infrastructure
- Collaboration
- Trust
- Sustainable technlology
- Solutions

### Terms (NEW)

- **TCO** - Total Cost of Ownership
- **CapEx** - Capital Expenditures - upfront costs
- **OpEx** - Operational Expenditures - running costs

### Regions and Timezones

- NA
- SA
- EU
- Middle East
- Africa
- Asia
- Australia

You can distribute different services in different regions/servers.

**Edge Network** - Stores popular user content. CDN?

If you store or configure it, you are responsible for securing it.

## Data

- How can data be structured? Some examples:
    - **Structured** : DBs, spreadsheets
    - **Semi-Structured** : JSON, XML, HTML
    - **Unstructured** : Text, posts, logs, and more. 

Structured data: Cloud SQL, Spanner, or BigQuery
Semi-structured data: Datastore and Bigtable.
Unstructured data: Cloud Storage

### Data Lifecycle Chain

Data Genesis -> Data Collection -> Data Processing -> Data Analysis -> Data Activation

Creation     -> Collecting      -> Filtering       -> What does it mean? -> The information in action

### Data Governance

- How is data stored, gathered, processed and disposed of?
- It makes the data available across the full lifecycle.
 
- **Benefits:**
    - Value
    - Cost controls
    - Regulatory compliance
    - Risk Management
    - Access

### **Unstructured Data** - Cloud Data Storage Classes

- **Standard** : "Hot" or frequently used data
- **Nearline** : Infrequently accesed, ~1x/mo access or less.  Some good examples are backups, long tail multimedia content or archived data
- **Coldline** : Very infrequent - cheaper. 
- **Archive Storage** : Lowest cost option. Data atchiving, online backup, disaster recovery. ~1x/year access.  Cheapest, minimum 365 day storage.

- **Autoclass** : A feature that categorizes and moves the object to the appropriate class based on acces pattern.

### **Structured Data** solutions:

- Relational Databases
- **Cloud SQL** - MySQL, PostgreSQL, SQL Server
    - Cloud SQL takes up the mundane tasks to let the customer focus on creating the application.
    - Is encrypted
    - Firewall
- **Spanner** - Relational database scales horizontally to handle business spikes.
    - Less downtime if instance becomes unavailable.
    - Redundancy
    - High availability
    - Will be more expensive
- **BigQuery** - Fully managed data warehouse
    - Built in ML
    - Analysis
    - Encrypted at rest by default
    - Eradicate data silos - works in multicloud environment
    - Can write models directly in BigQuery using SQL
    - Train ML modes and datasets with VertexAI integrated and easy export

### **Unstructured Data** solutions:

- **direstore**
    - Document storage
    - Automatic horizontal scaling
    - NoSQL
- **Bigtable**
    - Largeworkloads
    - Low Latency and bandwitdth
    - IoT, Analytics, Financial data analysis - think you need to process 1TB of data rapidly, or running ML on the data


### Workloads:

- Transactional - small, fast
- Analytical - read an entire dataset for processing, complex queries or aggregations
- CloudSQL for regional, Spanner for global

### Migrations:

- **Lift and shift**
    - Migrate from on-prem to public cloud
    - More difficult to modernize but less upheaval
- **Managed Migration**
    - Moves from SQL Server, MySQL, PostgreSQL to cloud

### Data Accessibility and Usability:

- **Looker**: Business Intelligence (BI) platform.
    - Analysis, Visualization, Share data
    - Dashboards and reports
    - Supports BigQuery and 60+ SQL dbs.

- **Streaming vs batch processing analytics**
    - Batch is traditional, streaming is good for small sized processed continuously (think in KBs), aka sensors, social media feeds, stock market quotes, app activity etc.
    - Real time data

### Data Stream services

- **Pub/Sub**
    - Distributed messaging
    - RECEIVES the data
- **Dataflow**
    - Processing the data (**ETL** - Extract, transform, load)
    - Apache Beam is a popular solution for pipeline design
    - Dataflow is serverless and fully managed, meaning more time analyzing insights, less time maintaining infra

## AI and ML

- **AI** - mimics cognitive functions
- **ML** - AI sub - Deep Learning Robotics, Expert Systems, NLP

#### Data Quality:

- Completeness
- Uniqueness
- Timeliness
- Validity
- Accuracy
- Consistency

## SECURITY

### Key Terms and Concepts:

**Confidentiality, Integrity, Availability - the CIA TRIAD**

- Confidentiality: Protecting privacy - only those with authority can access the appropriate data
- Integrity: Quality, accuracy and trustworthiness
- Availability: Making sure the data is accessible

**Control measures**: Processes implemented to manage and mitigate security risks. Eg. Auth, security training

### Google Infrastructure:

- All Google Cloud data is encrypted.
- Cloud Key Management Service (Cloud KMS) to self manage keys
- AES - Advanced Encryption Standard

### 3 A's - Authentication, Authorization, Auditing

- Auth - think username/password
- Authorization - privilages
- Auditing - tracking user activities

- **BeyondCorp Enterprise**: Zero trust model
- **VPC or Virtual Private Cloud** - secure your cloud
- **Cloud Armor** - DDOS potection
- **Terraform, Jenkins and Cloud Build** - handles all behind the scenes work
- **Google Cloud's Security Command Center (SCC)** - Overview for security posture
- **Cloud Logging** - collect and analyze security logs

## DevOps

- Developers write code
- Operators ensure operations run smoothly and reliably

- **SRE** - Site Reliablility Engineering
    - Service Level Indicators
        - Measurements
    - Service Level Objectives
        - Self imposed
    - Service Level Agreements
        - Agreement with the customer
- **Monitoring** - 
- **4 Golden Signlas**
    - Latency - Time to response
    - Traffic - Number of requests
    - Saturation - checks how close to capacity
    - Errors - Flaw/failure

- Infra needs to be resilient, fault tolenrant and scalable.

- Redundancy is for backup. Duplicating critical components to ensure redundant component can take over if needed
- Replication - multiple copies of data in different services or locations
- Regions - Allows other regions to take over if one fails 
- Scalability - Autoscales with demand
- Backups - 

