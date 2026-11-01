# Lab Environment

## Host
- Windows laptop running VMware
- **RAM:** 16 GB
- **Storage:** 512 GB SSD
- Git workflow: commits are made from the Kali VM and pushed to GitHub over SSH

## Virtual Machine
- **OS:** Kali Linux (rolling)
- **RAM:** 7.7 GB
- **Disk:** 79 GB
- **Docker:** 29.8.1
- **Docker Compose:** v5.5.1

## Services in the VM
| Service | Version | Ports |
|---|---|---|
| Wazuh manager / indexer / dashboard (single-node) | 4.7.5 | 443 (dashboard), 9200 (indexer), 55000 (API), 1514-1515 |
| OWASP crAPI (Docker) | latest | 8888 (web), 8443 (HTTPS), 8025 (MailHog), bound to 127.0.0.1 |
| MISP | latest | 8080, 4443 (stopped to free RAM while crAPI runs) |

## Notes
- The VM's RAM is limited, so unused containers (such as MISP) are stopped while crAPI and Wazuh run.
- No port conflicts between the Wazuh stack and crAPI.
