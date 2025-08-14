# TASK 7: Monitor System Resources Using Netdata

## Objective
Install and run **Netdata** to visualize real-time system and application performance metrics using Docker.

## Tools Used
- **Netdata** (Free, open-source monitoring tool)
- **Docker**

---

## Steps Followed

### 1. Run Netdata via Docker
```bash
docker run -d --name=netdata \
  -p 19999:19999 \
  --cap-add SYS_PTRACE \
  --security-opt apparmor=unconfined \
  netdata/netdata
