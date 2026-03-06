# Project-03-Linux-Server-Monitoring-using-Prometheus-and-Grafana
This project demonstrates how to build a complete monitoring stack for Linux servers using Prometheus, Node Exporter, and Grafana. The monitoring system collects real-time system metrics such as CPU usage, memory usage, disk utilization, and network statistics. Grafana dashboards provide visualization and help detect system performance issues.

**Flow**

Linux Server → Node Exporter → -Prometheus → Grafana Dashboard

⚙️ **Technologies Used**

- Linux (Ubuntu)

- Prometheus

- Node Exporter

- Grafana

- Shell Scripting

📊 **Features**

- Real-time monitoring of CPU, Memory, Disk, and Network

- Metrics collection using Node Exporter

- Data storage and scraping using Prometheus

- Interactive dashboards using Grafana

- Alert configuration for high CPU usage

🖥 **Installation Steps**
1. Install Node Exporter
   
```
wget https://github.com/prometheus/node_exporter/releases/latest/download/node_exporter-1.10.2.linux-amd64.tar.gz
tar -xvf node_exporter-*.tar.gz
cd node_exporter-*
./node_exporter
```
2. Install Prometheus

```
wget https://github.com/prometheus/prometheus/releases/latest/download/prometheus-3.10.0.linux-amd64.tar.gz
tar -xvf prometheus-*.tar.gz
cd prometheus-*
./prometheus --config.file=prometheus.yml
```
3. Install Grafana

```
sudo apt install grafana -y
sudo systemctl start grafana-server
```

Access Grafana:
```
http://SERVER_IP:3000
```

📈 Dashboard

Grafana dashboard shows:

- CPU Usage

- Memory Utilization

- Disk Usage

- Network Traffic

- System Load
