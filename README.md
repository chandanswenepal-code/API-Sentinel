\# API Sentinel



\*\*API Security Monitoring, Threat Detection and Incident Response Using SIEM\*\*



API Sentinel is a hands-on security project that simulates attacks against a deliberately vulnerable API (OWASP crAPI), forwards the resulting logs into a SIEM (Wazuh + OpenSearch), and walks through the full SOC workflow: detection, investigation, incident reporting and response.



\## System Architecture



!\[API Sentinel System Architecture](docs/architecture/system-architecture.png)



\*\*End-to-end flow:\*\* Attack Simulation → Log Collection → Detection → Investigation → Response



\## Tech Stack



\- \*\*Target application:\*\* OWASP crAPI (Docker)

\- \*\*Attack tooling:\*\* Python scripts, Burp Suite, Postman

\- \*\*Log forwarding:\*\* Filebeat / Logstash

\- \*\*SIEM:\*\* Wazuh + OpenSearch

\- \*\*Visualization:\*\* Wazuh Dashboard (Grafana optional)



\## Project Status



\- \[ ] Phase 1: Foundation and target application (crAPI)

\- \[ ] Phase 2: SIEM setup (Wazuh + OpenSearch)

\- \[ ] Phase 3: Log pipeline

\- \[ ] Phase 4: Attack simulation

\- \[ ] Phase 5: Detection rules and alerts

\- \[ ] Phase 6: Dashboards and investigation

\- \[ ] Phase 7: Incident reports and response

\- \[ ] Phase 8: Documentation and demo



\## Repository Structure



```

api-sentinel/

├── docs/               # Architecture, screenshots, environment notes

├── target-app/         # crAPI deployment

├── siem/               # Wazuh / OpenSearch setup

├── attacks/            # Attack scripts and test cases

├── detection-rules/    # Custom detection rules

├── dashboards/         # Dashboard exports

├── incident-reports/   # SOC incident reports

└── scripts/            # Helper scripts

```



\## Author



Chandan Yadav (\[@chandanswenepal-code](https://github.com/chandanswenepal-code))

