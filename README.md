# SEG-GRAFANA VISUALIZATIONS FROM SEG-PROMETHEUS SERVER

## Overview

Visualization of backend server metrics collected by Prometheus in Grafana. Grafana is a popular open-source analytics and monitoring platform, while Prometheus is a monitoring and alerting toolkit designed for reliability and scalability.

## Prerequisites

Before proceeding, ensure you have the following installed:

- [Grafana](https://grafana.com/get)
- [Prometheus](https://prometheus.io/download/)

## Setup Instructions

### 1. Install Grafana

Download and install Grafana by following the instructions on the [official Grafana website](https://grafana.com/get).

### 2. Install Prometheus

Download and install Prometheus by following the instructions on the [official Prometheus website](https://prometheus.io/download/).

### 3. Configure Prometheus

Make sure your Prometheus configuration includes the necessary settings for scraping targets. Here's an example configuration snippet:

```yaml
scrape_configs:
  - job_name: "example-job"
    static_configs:
      - targets: ["localhost:9090"]
```
