# DevOps Project — Step 1: Repo scaffold & CI (Starter)


This is a minimal starter repository for the DevOps end-to-end project.


## Included
- Simple Node.js app
- Dockerfile
- GitHub Actions CI workflow (CodeQL + test)

## Quick start (locally)
1. Install Node.js (v18+) and npm.
2. From repository root:
   ```bash
   cd app
   npm ci
   npm start
   ```
3. To build the Docker image:
   ```bash
   docker build -t devops-sample-app:local .
   docker run -p 8080:8080 devops-sample-app:local
   ```

## What we'll do next
- Verify CI runs on PRs
- Add container scanning (Trivy)
- Add Terraform skeleton for infra
