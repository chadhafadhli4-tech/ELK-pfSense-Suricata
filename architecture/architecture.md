# Network Security and Monitoring Architecture

## Overview

This internship project combines firewall monitoring,
intrusion detection, centralized log management,
and security event visualization.

## Main Components

- **pfSense:** Firewall and network traffic filtering.
- **Suricata:** Network intrusion detection and prevention.
- **Logstash:** Log collection and processing, where configured.
- **Elasticsearch:** Event indexing, storage, and search.
- **Kibana:** Security event visualization and analysis.
- **Metricbeat and Packetbeat:** System and network monitoring,
  where deployed and configured.

## Logical Data Flow

1. Network traffic passes through the monitored infrastructure.
2. pfSense applies firewall rules and generates logs.
3. Suricata inspects traffic and generates security alerts.
4. Configured log pipelines collect and process events.
5. Elasticsearch indexes the events.
6. Kibana provides dashboards and search capabilities.

## Security Considerations

- Do not publish credentials, tokens, or private keys.
- Remove sensitive IP addresses and company information
  from screenshots and configuration examples.
- Document only components and integrations verified
  in the actual internship environment.
