# Vortex Pulse - ⚽ Performance Pulse X Smart Sub Coach

### 🧠 AI-Powered Football Intelligence System

*A full-stack AI system that predicts player fatigue-based performance and recommends optimal substitutions using real-time analytics, machine learning, and modern MLOps tools.*

<br>

## 🚀 Project Summary

Vortex Pulse (**Performance Pulse X Smart Sub Coach**) is an end-to-end research and engineering project that fuses:

* 🎯 **Fatigue-based Player Performance Prediction** (Performance Pulse)
* ➸ **AI-driven Substitution Recommendation System** (Smart Sub Coach)

Built using **Python**, **FastAPI**, **PostgreSQL**, **JavaScript**, **MLflow**, and **Prometheus**, the system empowers coaches and analysts to make **data-driven matchday decisions**, integrating real-time monitoring, interactive dashboards, and explainable ML predictions.

<br>

## 🌟 Use Case

Football teams make crucial decisions based on instinct. This project bridges that gap by:

* Predicting **player performance decline** due to fatigue
* Recommending **when and who to substitute**
* Providing a full-stack, cloud-ready system with **real-time metrics**, **tracking**, and **visual insights**

<br>

## 🔧 Core Features

| Module                          | Description                                                                |
| ------------------------------- | -------------------------------------------------------------------------- |
| 🧠 Fatigue-Based Prediction     | ML model trained on historical stats to predict player performance decline |
| ➸ Smart Sub Coach               | Substitution logic engine based on fatigue, fouls, and live performance    |
| 📊 Frontend (JS)                | Interactive charts and timelines (e.g., player fatigue curves, sub impact) |
| ⚙️ Backend API (FastAPI)        | REST API exposing predictions and sub suggestions                          |
| 🗃️ Database (PostgreSQL)       | Stores match data, predictions, sub history                                |
| 🔀 Experiment Tracking (MLflow) | Tracks model versions, metrics, and hyperparameters                        |
| 📈 Monitoring (Prometheus)      | Real-time system monitoring and performance metrics                        |

<br>

## 🛠️ Tech Stack

| Layer         | Tools/Frameworks                                  |
| ------------- | ------------------------------------------------- |
| Programming   | Python, JavaScript                                |
| ML & Data     | Scikit-learn, XGBoost, Pandas, NumPy              |
| Deep Learning | TensorFlow, PyTorch (for potential video/NLP use) |
| API & Backend | FastAPI, PostgreSQL                               |
| Frontend      | JavaScript (Chart.js, D3.js)                      |
| DevOps/MLOps  | Docker, MLflow, Prometheus, GitHub Actions, DVC   |
| Cloud & Infra | AWS (EC2, S3), Terraform, Docker Compose          |
| Visualization | Tableau, Streamlit, Matplotlib, Seaborn           |

<br>

## 🧐 Model Architecture

* **Input Features**: minutes played, sprint distance, tackles, cards, previous match rating
* **Fatigue Score**: regression model output between 0–1
* **Performance Prediction**: classification (Good, Average, Poor) or rating (0–10)
* **Substitution Rule Engine**: combines fatigue + cards + match context

<br>

## 🗂️ Project Structure

```bash
🗁 Vortx_Pulse/
│
🗁 data/                     # Raw & processed player/match data
🗁 notebooks/               # Jupyter notebooks (EDA, modeling, deployment)
🗁 src/
├─ etl_pipeline.py
├─ fatigue_predictor.py
├─ substitution_engine.py
└─ api.py                 # FastAPI backend
🗁 dashboard/               # JS-based frontend (Chart.js)
🗁 db/                      # SQL scripts & PostgreSQL schema
🗁 mlflow/                  # MLflow tracking setup
🗁 monitoring/              # Prometheus + Grafana configs
🗁 models/                  # Saved models, tracked with DVC
🗁 infrastructure/          # Docker, Terraform, CI/CD (GitHub Actions)
🗁 reports/                 # Research PDFs and presentation slides
├─ dvc.yaml
├─ requirements.txt
├─ Dockerfile
├─ README.md
└─ app.py                     # (Optional) Streamlit demo
```

<br>

## 🧐 Sample Output

### Player Fatigue Prediction

```json
{
  "player": "Trent Alexander-Arnold",
  "fatigue_score": 0.78,
  "predicted_performance": "Average",
  "recommendation": "Monitor or Rest"
}
```

### Substitution Suggestion

```json
{
  "minute": 68,
  "sub_out": "Midfielder #8",
  "sub_in": "Midfielder #14",
  "reason": "Pass accuracy dropped from 88% → 62%, on yellow card, under press"
}
```

<br>

## 🧪 How to Run Locally

1. **Clone Repository**

```bash
git clone https://github.com/marknature/Vortex_Pulse.git
cd folder-name
```

2. **Install Dependencies**

```bash
pip install -r requirements.txt
```

3. **Run FastAPI Backend**

```bash
uvicorn src.api:app --reload
```

4. **Run Frontend**

```bash
cd dashboard
open index.html  # or use VSCode Live Server
```

5. **Launch MLflow UI**

```bash
mlflow ui
```

6. **Start Prometheus Monitoring**

```bash
docker-compose -f monitoring/prometheus-compose.yml up
```

<br>

---

<br>

## 🎓 Research Applications

* **Causal Inference**: Impact of fatigue on match performance
* **Hypothesis Testing**: Did late substitutions correlate with better outcomes?
* **Generative AI Potential**: Create synthetic training data for rare scenarios
* **SDoH Extension**: Adapt methodology to healthcare analytics

<br>

## 📊 Live Demos & Reports

* 📺 [Demo Video](#)
* 📊 [Tableau Dashboard Sample (link or screenshots)](https://public.tableau.com/)
* 📄 Research Paper: [`reports/PPxSC_Report.pdf`](#)

<br>

## 🔐 Compliance & Ethics

* Adheres to **FAIR data principles**
* Data governance considerations for expansion into **health/finance**
* Uses **ML explainability** techniques (e.g., SHAP, LIME)

<br>

## 🧠 Future Enhancements

* Add **pose detection** to track fatigue visually (MediaPipe)
* Build **mobile coaching assistant app** with push notifications
* Real-time **event stream processing** (Apache Kafka)
* Integrate with **wearable sensor data** for true biofeedback

<br>

---

<br>

## 👨‍💻 Author

**Mark Chindudzi**
AI&+ML Cloud Engineer Enthusiast | Data Scientist | AU'27 ♧ Merging Science with Imagination <br>
[GitHub](https://github.com/marknature)  |  [LinkedIn](https://www.linkedin.com/in/marknature-c)  |  [LinkTree](https://linktr.ee/marknature)

<br>

## 👥 Team (2-person team)

* **Mark Chindudzi** – Project Lead, Mentor, AI/ML Engineering, Data Scientist, Computer Scientist, Data&Video Analyst, Quality Assurance Tester, Researcher
* **Shallin T. Tariro** - Project Manager Assistant, Mentee, Software Engineer, Full-Stack Engineer, UI/UX Designer, Documentation Specialist Assistant

<br>

## 📄 License

This project is licensed. See [`LICENSE`](./LICENSE) for more information.

<br>

💡 *“Great football decisions are powered by great data. This project brings that vision to life.”*
