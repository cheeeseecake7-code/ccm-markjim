# Laboratory 07 - Cloud Operations Engineer

## Mission Overview
This laboratory focuses on establishing an observability baseline for a server before a major traffic surge. The goal is to monitor the host system, deploy a web application in a container, generate test traffic, and review logs and metrics to confirm that the infrastructure is healthy and capable of handling increased demand.

## Objectives
- Use Linux command-line tools to check CPU, memory, and disk health.
- Deploy an Nginx container and verify it serves traffic correctly.
- Simulate user requests and intentionally trigger an HTTP 404 error.
- Review logs to identify application behavior and investigate failures.
- Use real-time container metrics to verify efficient CPU and memory usage.
- Document findings in Markdown and maintain evidence in a portfolio repository.

## Monitoring Commands Executed
```bash
free -m

df -h

top

docker run -d --name client-website -p 8080:80 nginx:latest

curl http://localhost:8080
curl http://localhost:8080/hidden-admin-page

docker logs client-website

docker stats
```

## Skills Learned
- Reading system baselines for CPU, memory, and disk usage.
- Monitoring live resource consumption in Linux environments.
- Deploying and testing containerized web applications.
- Identifying application issues through access logs.
- Translating raw telemetry into readable operational documentation.
- Building professional cloud-computing portfolio evidence.
