# aws-lambda-tr
# Serverless React + Python API Starter

This project is a serverless web application starter with:
- React frontend (static, deploys to S3 with CloudFront)
- Python backend (API on AWS Lambda, fronted by API Gateway)
- DynamoDB for tag/index storage
- S3 for blob storage
- Cognito for authentication
- CI/CD with GitHub Actions

---

## Directories

- `/frontend` — React app
- `/backend` — Python Lambda functions (API)
- `/infra` — AWS infrastructure as code (SAM)
- `/.github/workflows` — CI/CD pipelines

---

## Deployment

- **Frontend:** Push to `main` → deploys to S3 static site bucket
- **Backend:** Push to `main` → deploys Python Lambda/API via AWS SAM

---

## Setup Overview

1. Configure AWS credentials as GitHub secrets (`AWS_ACCESS_KEY_ID`, `AWS_SECRET_ACCESS_KEY`, `AWS_REGION`)
2. Adjust parameters in `/infra/template.yaml` as needed
3. Push code to `main` to trigger CI/CD

---

## To Do

- Fill in `/frontend` and `/backend` with your app code
- Configure Cognito user pool/domain in AWS Console if needed (can be automated)
- (Optional) Extend CI/CD for preview branches, staging, etc.
