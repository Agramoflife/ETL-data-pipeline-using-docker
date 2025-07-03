# ETL Pipeline Using Docker

This project provides a Dockerized ETL pipeline that migrates data from an AWS RDS PostgreSQL database to an on-premise PostgreSQL database using a secure SSH tunnel. The migration is done in configurable batches and includes post-migration row-count verification.

---

## 🛠 Features

- SSH tunnel setup to securely access RDS
- Batch-wise data migration using pandas
- Source and destination row count verification
- Dockerized setup for easy deployment
- Environment-based configuration
- Logging to both console and file


## ⚙️ Prerequisites

- Docker and Docker Compose installed
- Python 3.8+ (if running locally)
- SSH private key with access to the RDS server
- PostgreSQL credentials for RDS and on-premise

---

## 🔧 Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/your-username/ETL-pipeline-using-docker.git
cd ETL-pipeline-using-docker
```
Copy the sample environment file and update the values:
Add your private key file to the keys/ directory as specified in .env

To start the migration:
docker-compose up

To run the migration in the background
docker-compose up -d

Deepu Kumar
Data Scientist @ ElixirAI
