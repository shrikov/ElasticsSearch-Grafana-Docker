# Elasticsearch & Grafana Docker Stack

A simple monitoring stack with Elasticsearch and Grafana running on Docker for Red Hat Linux.

## Quick Start

```bash
# Clone the repository
git clone https://github.com/sherif/Elasticsearch-Grafana-Docker.git
cd Elasticsearch-Grafana-Docker

# Create data directories
mkdir -p elasticsearch-data grafana-data

# Set permissions
sudo chown -R 1000:1000 elasticsearch-data
sudo chown -R 472:472 grafana-data

# Start the stack
docker compose up -d

Connect Grafana to Elasticsearch
Open Grafana: http://localhost:3000
Login: admin / grafana123

Add data source → Elasticsearch

URL: http://elasticsearch:9200
Basic Auth: elastic / changeme
Click Save & Test
