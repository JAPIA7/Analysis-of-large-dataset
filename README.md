````markdown
# Social Media Trend Analysis System

A distributed big data analytics platform for analyzing social media engagement, virality, and trending patterns across multiple platforms using Apache Spark, Streaming Analytics, Machine Learning, and FastAPI.

## Platforms Analyzed
- Twitter
- TikTok
- Instagram
- YouTube
- Facebook

## Key Features
- Real-time trend analysis
- Engagement classification
- Streaming analytics
- Viral trend forecasting
- Drift monitoring
- Machine learning predictions
- REST API deployment

## Architecture
The system follows a Lambda Architecture:
- Batch Layer
- Speed Layer
- Serving Layer

## Technologies Used
| Technology | Purpose |
|---|---|
| Python 3.10 | Core programming |
| Apache Spark | Distributed processing |
| PySpark | Spark integration |
| FastAPI | API deployment |
| Spark MLlib | Machine learning |
| Structured Streaming | Real-time analytics |
| Parquet | Optimized storage |

## Machine Learning Models
- Logistic Regression
- Random Forest
- Gradient Boosted Trees

### Best Model Performance
- Accuracy: ~83%
- F1 Score: ~82%

## Research Innovation
### Adaptive Threshold Engine (ATE)
A custom classification engine that dynamically adjusts engagement thresholds per platform instead of using one global threshold.

**Improvement:** +5% to 12% classification accuracy.

## Dataset
The dataset contains:
- Likes
- Shares
- Comments
- Views
- Platform
- Content Type
- Region
- Timestamp
- Virality Score

### Dataset Size
- 10,000+ synthetic records
- Scalable to millions of records

## Project Structure
```bash
project/
├── data/
├── models/
├── reports/
├── logs/
├── src/
├── run_pipeline.py
├── requirements.txt
└── README.md
````

## API Endpoints

| Endpoint            | Description       |
| ------------------- | ----------------- |
| GET /health         | Health check      |
| GET /metrics        | Model metrics     |
| POST /predict       | Single prediction |
| POST /predict/batch | Batch prediction  |
| GET /monitor/drift  | Drift monitoring  |

## Running the Project

### Clone Repository

```bash
git clone [YOUR_GITHUB_LINK]
cd project
```

### Create Virtual Environment

```bash
py -3.10 -m venv venv
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run Pipeline

```bash
python run_pipeline.py --milestone 1
```

### Start API

```bash
python src/deployment/serve.py --api
```

API URL:

```bash
http://localhost:8000
```

Swagger Docs:

```bash
http://localhost:8000/docs
```

## Challenges Solved

| Challenge                             | Solution                      |
| ------------------------------------- | ----------------------------- |
| PySpark incompatible with Python 3.11 | Used Python 3.10              |
| JAVA_HOME errors                      | Configured OpenJDK 11         |
| Kafka unavailable locally             | Simulated streaming           |
| Slow Spark inference                  | Lightweight prediction engine |

## System Performance

| Metric            | Result      |
| ----------------- | ----------- |
| Streaming Latency | < 5 seconds |
| API Response Time | < 50ms      |
| Best F1 Score     | ~0.82       |
| ATE Improvement   | +5% to 12%  |

## Conclusion

This project demonstrates a complete large-scale analytics system combining:

* Big data engineering
* Distributed computing
* Streaming systems
* Machine learning
* REST API deployment
* Intelligent adaptive analytics

The platform supports both historical and real-time social media trend analysis at scale.


