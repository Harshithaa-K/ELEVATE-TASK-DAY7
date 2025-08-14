# TASK 7: Monitor System Resources Using Netdata

## Objective
Install and configure **Netdata** to monitor system performance metrics in real time, including CPU, memory, disk usage, and Docker containers.

---

## Tools Used
- **Netdata** – Open-source, real-time monitoring tool
- **Docker** – To run Netdata in a container
- **Ubuntu (WSL2)** – Environment where Netdata is installed

---

## Installation & Setup

### 1️⃣ Pull and Run Netdata via Docker
docker run -d \
  --name=netdata \
  -p 19999:19999 \
  --cap-add SYS_PTRACE \
  --security-opt apparmor=unconfined \
  netdata/netdata


2️⃣ Access the Netdata Dashboard
http://localhost:19999

## Logs Location

docker exec -it netdata bash
cd /var/log/netdata
ls

Note:
## Screenshots are attached in the repository
