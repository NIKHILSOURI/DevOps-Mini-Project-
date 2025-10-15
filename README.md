# DevOps Mini Project – ML Inference Deployment using Docker and Jenkins CI/CD

## 🧩 Overview
This project demonstrates how to automate an **ML inference pipeline** using **Docker** and **Jenkins**, deploying it seamlessly on **AWS EC2**.  
The pipeline automates container build, deployment, and testing stages—reducing manual work and achieving up to **60% faster deployment cycles**.

---

## ⚙️ Tech Stack
- **Languages:** Python  
- **Tools:** Docker, Jenkins, AWS EC2  
- **Libraries:** scikit-learn, pandas, joblib  
- **Concepts:** CI/CD, Containerization, Model Deployment, MLOps  

---

## 🚀 Workflow

1. **Model Preparation**  
   - A lightweight ML model is trained and serialized using `joblib`.
   - Input: preprocessed dataset → Output: model + test metrics.

2. **Containerization with Docker**  
   - The model and inference script are packaged into a Docker image.
   - Dependencies are defined in the `Dockerfile`.

3. **Deployment to AWS EC2**  
   - The Docker image is built and deployed to an EC2 instance.  
   - Ensures consistent runtime across environments.

4. **Automation via Jenkins**  
   - Jenkins pipeline triggers automatically on Git commits.  
   - Steps include:
     - **Build Stage:** Build Docker image  
     - **Deploy Stage:** Run the container on EC2  
     - **Test Stage:** Execute inference & log metrics  

