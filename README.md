# Cybersecurity Portfolio 1 (P1) — Homelab Build, Telemetry, & Case Files

## Overview
This portfolio documents a practical security lab environment and the workflows built on top of it:
- segmented network design (Proxmox + pfSense)
- centralized Windows telemetry (WEF + Sysmon)
- investigation-style case files and detection artifacts (Splunk / Elastic / Wazuh)

## Sanitization Note
This portfolio uses representative hostnames/IP ranges and redacts WAN/public IPs, domains/DDNS, VPN details, and secrets. Architecture and workflow remain accurate.

---

## Featured Projects (P1)

### 1) P1-1: Proxmox Segmentation Lab (Foundation)
**Repo:** `P1-1-proxmox-segmentation-lab`  
**What it is:** segmented Proxmox + pfSense blueprint with VM inventory, firewall posture, and safe publishing guidelines.  
**Why it’s included:** establishes the lab design used by all other P1 projects.
- Key artifacts: architecture, bridges, firewall policy, IP plan, VM inventory

Repo: https://github.com/kvntynito/P1-1-proxmox-segmentation-lab

---

### 2) P1-2: Telemetry Pipeline (WEF + Sysmon → Wazuh / Elastic / Splunk)
**Repo:** `P1-2-wef-sysmon-to-wazuh-elastic-splunk`  
**What it is:** blueprint for centralized Windows telemetry collection and multi-platform validation.  
**Why it’s included:** builds SOC-style telemetry flow and repeatable validation checks.

Repo: https://github.com/kvntynito/P1-2-wef-sysmon-to-wazuh-elastic-splunk

---

### 3) P1-3: Incident Investigation Case Files
**Repo:** `P1-3-incident-investigation-casefiles`  
**What it is:** case templates + detections folders (Splunk searches / Elastic queries / Wazuh notes) tied to lab telemetry.  
**Why it’s included:** documents investigation workflow (timeline, IOCs, pivots) with sanitized evidence.

Repo: https://github.com/kvntynito/P1-3-incident-investigation-casefiles

---

## How the projects connect
- **P1-1** provides the segmented lab foundation (networks, firewall boundaries, VM layout)
- **P1-2** uses that lab to centralize endpoint telemetry (WEF + Sysmon)
- **P1-3** uses that telemetry to build repeatable investigations and detection artifacts

## Current Status
Blueprint phase complete. Evidence (screenshots + implementation notes) will be added as each milestone is implemented in the homelab.
