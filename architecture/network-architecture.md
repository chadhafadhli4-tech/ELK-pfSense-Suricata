# Network Security and Monitoring Architecture

This diagram illustrates the logical architecture of the internship project.

```mermaid
flowchart TD
    A["Network Traffic"] --> B["pfSense Firewall"]
    B --> C["Suricata IDS/IPS"]
    B --> D["Firewall Logs"]
    C --> E["Security Alerts"]
    D --> F["Logstash"]
    E --> F
    F --> G["Elasticsearch"]
    G --> H["Kibana Dashboards"]
```

## Components

- **pfSense:** Firewall and network traffic filtering.
- **Suricata:** Network intrusion detection and prevention.
- **Logstash:** Log collection and processing.
- **Elasticsearch:** Event indexing and storage.
- **Kibana:** Log visualization and analysis.

*The diagram represents the logical architecture. Actual log flows depend on the integration configured during the internship.*
