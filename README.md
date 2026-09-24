# DevOps Infrastructure Project

Educational DevOps project created to practice infrastructure automation, containerization, orchestration, monitoring, CI/CD, and Git workflows.

## Project Structure

- `terraform/` — Terraform infrastructure configuration and variables.
- `ansible/` — Ansible playbook for configuration management.
- `docker/` — Dockerfile for building the application container.
- `kubernetes/` — Kubernetes Deployment and Service manifests.
- `monitoring/` — Prometheus monitoring configuration.
- `.github/workflows/` — GitHub Actions CI workflow.
- `.gitignore` — files and directories excluded from Git.
- `README.md` — project documentation.

## Technologies

- Git and GitHub
- Terraform
- Ansible
- Docker
- Kubernetes
- Prometheus
- GitHub Actions

## Docker

The Dockerfile uses Python 3.11 and runs a simple Python command inside the container.

Build the image:

docker build -t devops-project ./docker

Run the container:

docker run --rm devops-project

## Kubernetes

The Kubernetes configuration contains:

- Deployment with 2 replicas
- nginx:alpine container
- Service using port 80

## Monitoring

Prometheus is configured to collect metrics every 15 seconds.

## CI/CD

GitHub Actions runs automatically on pushes and pull requests to the main branch.

The workflow:

1. Checks out the repository.
2. Builds the Docker image.
3. Runs the Docker container.

## Git Workflow

The project uses feature branches and Pull Requests.

During development, multiple feature branches were created and merged into main. A merge conflict in README.md was intentionally created and manually resolved as part of Git practice.
