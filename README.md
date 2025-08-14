# Task 7: Monitor System Resources Using Netdata

## Objective
Install Netdata via Docker and visualize system/app performance metrics.

## Tools
- Netdata (Docker image: `netdata/netdata`)
- Docker

## Steps
## 1. Pull & Run Netdata

   ```bash
   docker run -d --name=netdata \
     -p 19999:19999 \
     --cap-add SYS_PTRACE \
     --security-opt apparmor=unconfined \
     netdata/netdata
     
```
## 2. Access Dashboard: Visit http://localhost:19999

## 3. Monitor Metrics: CPU, memory, disk, network, Docker containers.

## 4. Check Logs: Inside /var/log/netdata in the container.