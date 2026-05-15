# Docker Multi-Stage Builds

> Reduce Docker image sizes by 70-95% using multi-stage builds

## Results

| Language | Before | After  | Reduction |
|----------|--------|--------|-----------|
| Python   | 1.2 GB | 180 MB | 85%       |
| Node.js  | 980 MB | 120 MB | 88%       |
| Go       | 800 MB |  15 MB | 98%       |

## How to use

Clone the repo and build:
  docker build -t myapp -f python/Dockerfile .
  docker images myapp

## Key techniques
- Separate build and runtime stages
- Alpine/slim base images for production
- .dockerignore to exclude dev files
