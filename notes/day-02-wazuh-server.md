# Day 2: Wazuh Server Deployment

## Objective

Deploy and secure a dedicated Wazuh server for the SOC home lab.

## Environment

- Hypervisor: VMware Workstation
- Deployment: Official Wazuh OVA
- Wazuh version:
- Host RAM: 16 GB
- VM RAM: 8 GB
- VM CPU allocation: 4 cores
- VM storage: 50 GB
- Network mode: NAT
- Server private IP: [sanitized or omitted]

## Validation

- Wazuh manager: Active
- Wazuh indexer: Active
- Wazuh dashboard: Active
- Filebeat: Active
- Dashboard accessible from second computer: No

## Security Measures

- Changed the default Linux account password
- Changed the default Wazuh dashboard administrator password
- Kept the dashboard restricted to the private home network
- Did not configure internet-facing port forwarding

## Challenges and Solutions

I could not open my wazuh virtual machine for hours and found out it was due to my virtual
machine not being updated to the lastest model.

## Next Step

Create a Windows virtual endpoint and deploy the Wazuh agent.