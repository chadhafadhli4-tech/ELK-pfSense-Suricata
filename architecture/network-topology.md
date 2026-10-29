# Network Topology

## Overview

This document describes the virtual cybersecurity lab used
for centralized logging, network monitoring and intrusion detection.

## Components

| Component | Role |
|---|---|
| pfSense | Firewall and network traffic filtering |
| Elasticsearch | Log storage and search |
| Logstash | Log processing and ingestion |
| Kibana | Log visualization and dashboards |
| Suricata | Network intrusion detection and prevention |
| Metricbeat | System metrics collection |
| Packetbeat | Network traffic monitoring |

## Network

The lab uses virtual network interfaces and private IP addressing.

The actual IP addresses, network interfaces and communication
paths must be verified against the running lab before deployment.

## Data Flow

1. Network devices and systems generate logs.
2. Logs are forwarded to the configured collection pipeline.
3. Logstash processes incoming events where configured.
4. Elasticsearch indexes the events.
5. Kibana displays searchable logs and dashboards.
6. Suricata can generate security alerts when integrated.

## Security

Never publish passwords, private keys, API tokens or confidential logs.
