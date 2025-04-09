# 🚀 Real-Time Data Pipeline with Kafka, Airflow & PostgreSQL

This project showcases a robust, production-grade data pipeline capable of real-time ingestion, transformation, validation, and storage using tools like **Kafka**, **PostgreSQL**, **Apache Airflow**, and **Docker**.

---

## 🧩 Features
- Real-time data ingestion using **Kafka**
- Batch & streaming support
- Schema validation and transformation
- Star schema-based data modeling (fact/dimension tables)
- Database output via **SQLAlchemy** to PostgreSQL
- Orchestration with **Apache Airflow**
- Testing with **pytest** (unit, integration, E2E)
- Data security via encryption and masking
- Dockerized setup for portability

---

## 📁 Project Structure
```
├── data_pipeline.py              # Main pipeline script
├── kafka_producer_simulator.py  # Simulated Kafka producer
├── data_validation.py           # Schema validation logic
├── star_schema.sql              # Star schema DDL
├── test/                        # Unit & integration tests
├── dags/                        # Airflow DAG definitions
├── Dockerfile                   # Docker configuration
├── Makefile                     # Helper commands
├── requirements.txt             # Python dependencies
└── README.md                    # Documentation
```

---

## ⚙️ Setup & Usage

### 🔧 Local Setup
```bash
make setup
```

### ▶️ Run the Pipeline
```bash
make run-pipeline
```

### ✅ Run Tests
```bash
make run-tests
```

### 🧪 Simulate Kafka Stream
```bash
make run-kafka-producer
```

### 🐳 Docker
```bash
make build-docker
make run-docker
```

### 🧠 Load Schema
```bash
make load-schema
```

---

## 🧪 Testing Strategy
- Unit tests for transformation and validation functions
- Integration test for database connectivity
- End-to-end tests for full pipeline verification

---

## 📊 Technologies Used
- Python, Pandas, SQLAlchemy
- Kafka (via `kafka-python`)
- PostgreSQL
- Apache Airflow
- Docker, Make
- pytest, cryptography

---

## 📌 Assumptions
- PostgreSQL is accessible locally or via Docker
- Kafka is available at `localhost:9092`
- Python 3.8+ is used

---

## 📄 License
MIT

