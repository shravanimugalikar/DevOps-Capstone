# DevOps Capstone App

## Overview
Simple Flask application with health endpoint.

## Architecture
Developer
    |
    v
 GitHub Repository
    |
    v
 GitHub Actions
(Build + Test)
    |
    v
 Docker Container
    |
    v
 Flask App
(/ and /health)

## Local Run
python app.py

## Docker
docker build -t devops-pulse:1.0 .
docker run -p 8080:8080 devops-pulse:1.0

## CI/CD
GitHub Actions runs tests and Docker build.

## Monitoring
CloudWatch (planned for deployment phase).

## Cleanup
Delete resources after testing.
