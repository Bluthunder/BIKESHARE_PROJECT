# 🚴‍♂️ Bike Share Rental Project 🚴‍♀️  
![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/your-repo/model_pipeline.yaml?style=for-the-badge)  
![Python](https://img.shields.io/badge/Python-3.10-blue?style=for-the-badge&logo=python)  
![FastAPI](https://img.shields.io/badge/FastAPI-🚀-green?style=for-the-badge)  
![Docker](https://img.shields.io/badge/Docker-🛳️-blue?style=for-the-badge)  

A **Machine Learning model training and deployment pipeline** for a **Bike Share Rental System**. This project automates the entire ML workflow, from training to API deployment using **GitHub Actions, FastAPI, Docker, and Pytest**.



## 🏗️ Project Structure  
```bash
📂 BIKESHARE_PROJECT
│-- .github/workflows/model_pipeline.yaml  # CI/CD Pipeline  
│-- bike_sharing_api/                      # API Code  
│-- bikeshare_model/                        # ML Model Code  
│-- requirements/                           # Dependencies  
│-- tests/                                  # Unit Tests  
│-- dist/                                   # Built Packages  
│-- setup.py                                # Package Setup  
│-- README.md                               # This File  


⚡ Features
✅ Automated Model Training (CatBoost, Sklearn, etc.)
✅ Unit Testing & CI/CD with GitHub Actions
✅ API Deployment with FastAPI & Docker
✅ Model Packaging into a .whl file


🚀 Installation & Usage

1️⃣ Clone the Repository
```bash
git clone https://github.com/your-repo.git
```
cd BIKESHARE_PROJECT

2️⃣ Install Dependencies
```bash
pip install -r requirements/requirements.txt
```

3️⃣ Train the Model
```bash
python bikeshare_model/train_pipeline.py
```

4️⃣ Run Unit Tests
```bash
pytest tests/
```

5️⃣ Build and Run the API Locally
```bash
docker build -t bikesharing-api .
docker run -p 8000:8000 bikesharing-api
```

API will be available at 👉 http://localhost:8001

🏗️ GitHub Actions Workflow
The CI/CD pipeline automates the following:
✔️ Setup & Dependency Installation
✔️ Model Training & Artifact Upload
✔️ Unit Testing
✔️ Building & Pushing Docker Image

📜 License
📄 This project is licensed under the MIT License.

🤝 Contributing
🙌 PRs & Issues are welcome! Follow the contributing guidelines.

📬 Contact
📧 Your Name – Kaushik T D Roy
🐦 Twitter – @kaushiktd
🔗 LinkedIn – https://www.linkedin.com/in/kaushiktd/