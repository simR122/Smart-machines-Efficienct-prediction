# Smart Manufacturing Machine Efficiency Prediction

![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)
![GitHub](https://img.shields.io/badge/GitHub-Version_Control-black?logo=github)
![Google Cloud Platform](https://img.shields.io/badge/GCP-Cloud_Platform-blue?logo=google-cloud)
![Python](https://img.shields.io/badge/Python-Programming_Language-blue?logo=python)
![HTML](https://img.shields.io/badge/HTML-Markup_Language-orange?logo=html5)
![CSS](https://img.shields.io/badge/CSS-Styling-blue?logo=css3)
![Pandas](https://img.shields.io/badge/Pandas-Data_Analysis-green?logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Scientific_Computing-blue?logo=numpy)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-Machine_Learning-orange?logo=scikit-learn)
![Flask](https://img.shields.io/badge/Flask-Web_Framework-black?logo=flask)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Data_Visualization-blue)
![Docker](https://img.shields.io/badge/Docker-Containerization-blue?logo=docker)
![Kubernetes](https://img.shields.io/badge/Kubernetes-Orchestration-blue?logo=kubernetes)
![Jenkins](https://img.shields.io/badge/Jenkins-CI-red?logo=jenkins)
![Minikube](https://img.shields.io/badge/Minikube-Kubernetes_Local-orange?logo=kubernetes)
![ArgoCD](https://img.shields.io/badge/ArgoCD-Deployment-blue?logo=argo)

## Dataset [Kaggle LINK](https://www.kaggle.com/datasets/ziya07/smart-manufacturing-iot-cloud-monitoring-dataset)

## Overview
This project predicts the efficiency of smart manufacturing machines using machine learning. It includes a Flask-based web application for user interaction and a CI/CD pipeline for deployment.

## Features
- **Machine Learning Model**: Predicts machine efficiency based on various input features.
- **Flask Web App**: User-friendly interface for predictions.
- **CI/CD Pipeline**: Automated build, test, and deployment using Jenkins, Docker, and ArgoCD.
- **Kubernetes Orchestration**: Manages containerized applications.


## Workflow
Below is the workflow for the project:

![Workflow](static/workflow_diagram.png)

## How to Run the Project
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/data-guru0/GITOPS-PROJECT-9.git
   cd GITOPS-PROJECT-9
   ```

2. **Set Up the Environment**:
   - Install dependencies using `setup.py`:
     ```bash
     python setup.py install
     ```

3. **Run the Flask App**:
   ```bash
   python application.py
   ```
   Access the app at `http://localhost:5000`.

4. **Build and Deploy with Docker**:
   - Build the Docker image:
     ```bash
     docker build -t smart-machine-efficiency .
     ```
   - Run the container:
     ```bash
     docker run -p 5000:5000 smart-machine-efficiency
     ```

5. **CI/CD Pipeline**:
   - Use the provided `Jenkinsfile` for automated builds and deployments.

## Input Features
The model uses the following features for predictions:
- Operation Mode
- Temperature (°C)
- Vibration (Hz)
- Power Consumption (kW)
- Network Latency (ms)
- Packet Loss (%)
- Quality Control Defect Rate (%)
- Production Speed (units/hr)
- Predictive Maintenance Score
- Error Rate (%)
- Date and Time (Year, Month, Day, Hour)

## Deployment
- **Kubernetes**: Use the provided manifests for deploying the app.
- **ArgoCD**: Sync the app with ArgoCD for continuous deployment.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing
Contributions are welcome! Please open an issue or submit a pull request.
