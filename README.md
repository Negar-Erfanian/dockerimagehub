# Docker Image Hub – CI/CD for Flask App

This repository demonstrates end-to-end **CI/CD workflows for Flask App**, including automated testing, Docker image building, and container registry deployment. It showcases practical skills in cloud-native deployment and modern DevOps practices.

## Features

- **Flask-Based Service**: A very simple "Hello World" app.
- **Automated CI/CD Pipelines**: Implemented using GitHub Actions to:
  - Run unit and integration tests
  - Build Docker images
  - Push images to container registries
- **Containerization**: Fully containerized service using Docker for consistent environments.
- **Cloud Deployment Ready**: Designed for seamless deployment to cloud platforms (AWS, Azure, GKE).

## Project Structure
```
dockerimagehub/
├── app.py         # Flask API entry point
├── requirements.txt # Python dependencies
├── test_app.py/   # Test Cases
├── .github/workflows/
│   └── ci-cd.yml       # GitHub Actions workflow
├── Dockerfile           # Docker build configuration
└── README.md
```

## How It Works

1. **Local Development**
   - Install dependencies:
     ```bash
     pip install -r requirements.txt
     ```
   - Run the service locally:
     ```bash
     python app.py
     ```
   - Test API endpoints using Postman or curl.

2. **CI/CD Pipeline**
   - Every push to the repository triggers GitHub Actions:
     - Runs automated tests
     - Builds Docker image
     - Pushes image to the specified container registry

3. **Deployment**
   - The built Docker image can be deployed to any cloud environment, including AWS ECS, Azure Container Instances, or Google Kubernetes Engine (GKE).

## Skills Demonstrated

- Containerization
- Flask API development
- CI/CD automation using GitHub Actions
- Docker image management and registry deployment
- Cloud-native deployment practices

## Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/Negar-Erfanian/dockerimagehub.git
   cd dockerimagehub
   ```
   
2. Build the Docker image:
  ```bash
  docker build -t dockerimagehub:latest .
```

3. Run the container locally:
    ```bash
    docker run -p 5000:9000 dockerimagehub:latest
    ```

4. Access the API:
```bash
http://localhost:9000/predict
```
