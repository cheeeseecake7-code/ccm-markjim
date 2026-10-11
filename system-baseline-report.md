# System Baseline Report

## Host Resource Check
The server baseline was reviewed before deploying the application to understand whether the physical host had enough capacity to support a heavy workload.

### Recorded Values
- Total RAM available on the server: 7.7 GiB
- Total storage capacity of the root (/) filesystem: 50G

### Baseline Observations
- Memory usage and available memory were checked using `free -m`.
- Disk usage was reviewed using `df -h` to confirm available storage on `/`.
- CPU load and running processes were observed in `top` to confirm the system was not already saturated.

### Why Disk Space Matters Before Traffic Surge
Checking disk space is critical before a large traffic surge because a full or nearly full filesystem can cause application instability, failed log writes, slowdowns, and unplanned outages when demand spikes.

### Evidence
Screenshots for the baseline checks were saved in the `screenshots/` folder as:
- `memory-check.png`
- `disk-check.png`
