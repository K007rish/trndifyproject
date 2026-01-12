# Trend Application – DevOps Deployment

## Stack Used
- Docker
- Jenkins
- Terraform
- AWS EC2
- AWS EKS
- Kubernetes
- Prometheus & Grafana

## CI/CD Flow
1. GitHub commit push triggers Jenkins
2. Jenkins builds Docker image
3. Image pushed to DockerHub
4. Deployed to EKS using kubectl
5. App exposed via LoadBalancer

## Access Application
```bash
kubectl get svc trend-service
