# ComputerVitals

A monitoring stack for computer health and Docker container statistics using Prometheus, Grafana, cAdvisor, and Node Exporter.

## Quick Start

1. Start the containers:
   ```bash
   docker compose up -d
   ```

2. Access the services:
   - Grafana: http://localhost:3000
   - Prometheus: http://localhost:9090
   - cAdvisor: http://localhost:8080
   - Node Exporter: http://localhost:9100

## Setup Instructions

### 1. Grafana Login
- URL: http://localhost:3000
- Default Credentials: `admin` / `admin`

### 2. Connect Prometheus
1. Go to **Connections** > **Data Sources**.
2. Click **Add data source** and select **Prometheus**.
3. Set the URL to: `http://prometheus:9090`
4. Click **Save & Test**.

### 3. Import Dashboard
1. Go to **Dashboards** > **New** > **Import**.
2. Use ID `14282` (Docker metrics) or `1860` (Host metrics).
3. Select the **Prometheus** data source and click **Import**.
