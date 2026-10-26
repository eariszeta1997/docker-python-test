# Docker Python Test Environment

A lightweight development environment setup running a containerized Python web server on **WSL2 (Ubuntu)** with **Docker** and **VS Code**.

## Stack
- **OS**: Windows 10 Host + WSL2 (Ubuntu)
- **Container Runtime**: Docker Desktop
- **Runtime**: Python 3.11-slim
- **Editor**: Visual Studio Code

## Getting Started

### 1. Build the Docker image
```bash
docker build -t mio-server-test .
```

### 2. Run the container
```bash
docker run -d -p 8080:8080 --name test-app mio-server-test
```

### 3. Verify
Open your browser and navigate to:
```
http://localhost:8080
```
