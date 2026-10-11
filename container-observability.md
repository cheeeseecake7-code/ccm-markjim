# Container Observability Report

## Application Log Evidence
The application log line showing the HTTP 404 error is:

```text
172.17.0.2 - - [11/Oct/2026:12:45:31 +0000] "GET /hidden-admin-page HTTP/1.1" 404 153 "-" "curl/8.0.1"
```

Application logs are vital for troubleshooting because they show exactly which requests failed, when they failed, and what response code the client received. This evidence helps engineers identify broken routes, misconfigurations, and user-facing issues without guessing.

## Real-Time Container Metrics
During the `docker stats` observation, the `client-website` container showed the following resource usage:

- Memory Usage: 3.5MiB
- CPU Percentage: 0.03%

### Evidence
The live metrics screenshot was saved in the `screenshots/` folder as:
- `container-metrics.png`
- `docker-logs.png`
