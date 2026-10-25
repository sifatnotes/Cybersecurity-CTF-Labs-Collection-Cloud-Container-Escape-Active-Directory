# Cybersecurity-CTF-Labs-Collection-Cloud-Container-Escape-Active-Directory
A curated index of hands-on cybersecurity labs covering Kerberos roasting, Docker container escapes, Kubernetes misconfigurations, and cloud credential leaks from Learn SecByte.
# Cloud, Container Escape & Active Directory CTF Labs Collection

A structured, searchable index of hands-on cybersecurity labs focusing on Active Directory Kerberos roasting, Docker container escapes, Kubernetes cluster compromise, and cloud credential leakage hosted on Learn SecByte.

This collection is designed for security engineers, CTF players, DevOps/DevSecOps teams, cloud security analysts, and penetration testers learning real-world cloud and infrastructure attack vectors.

---

## Table of Contents
- [Introduction](#introduction)
- [Lab Collection & Index](#lab-collection--index)
- [Categories](#categories)
  - [Active Directory & Kerberos Attacks](#active-directory--kerberos-attacks)
  - [Container Security & Docker Breakouts](#container-security--docker-breakouts)
  - [Kubernetes & Cloud Infrastructure Security](#kubernetes--cloud-infrastructure-security)
- [Learning Path](#learning-path)
- [How to Use the Labs](#how-to-use-the-labs)
- [Disclaimer](#disclaimer)

---

## Introduction

Modern infrastructure security demands expertise spanning enterprise Active Directory domains, container runtime isolation, container orchestration platforms, and cloud access controls. Securing hybrid environments requires practical knowledge of how misconfigurations allow attackers to extract credentials, escape containers, and compromise cloud resources.

This repository organizes hands-on security labs from Learn SecByte into structured learning paths for cloud, container, and directory security.

---

## Lab Collection & Index

| Lab Title | Domain / Category | Target Platform | Access Link |
| :--- | :--- | :--- | :--- |
| **AS-REP Roasting** | Active Directory | Windows / Kerberos | [Access Lab](https://learn.secbyte.org/ctf/as-rep-roasting-kerberos-preauth-abuse-detection) |
| **Kerberoasting** | Active Directory | Windows / Kerberos | [Access Lab](https://learn.secbyte.org/ctf/kerberoasting-from-kerberos-basics-to-ticket-abuse-detection) |
| **Container Secrets Exposure** | Container Security | Docker / Runtime | [Access Lab](https://learn.secbyte.org/ctf/container-secrets-exposure) |
| **Root Containers** | Container Security | Linux Containers | [Access Lab](https://learn.secbyte.org/ctf/root-containers) |
| **Host Namespace Escape** | Container Breakout | Linux / Docker | [Access Lab](https://learn.secbyte.org/ctf/host-namespace-escape) |
| **Kubernetes Misconfigurations** | Orchestration Security | Kubernetes / K8s | [Access Lab](https://learn.secbyte.org/ctf/kubernetes-misconfigurations-from-pod-to-cluster-compromise) |
| **Container Escape Breakout** | Container Breakout | Linux / Runtime | [Access Lab](https://learn.secbyte.org/ctf/container-escape-linux-container-breakout) |
| **Mounted Docker Socket** | Container Breakout | Docker Engine | [Access Lab](https://learn.secbyte.org/ctf/mounted-docker-socket-container-breakout-to-host-control) |
| **Privileged Containers Abuse** | Container Security | Docker / Capabilities | [Access Lab](https://learn.secbyte.org/ctf/privileged-containers-from-misconfiguration-to-detection) |
| **Docker Escape to Host** | Container Breakout | Docker Engine | [Access Lab](https://learn.secbyte.org/ctf/docker-escape-from-container-to-host-2) |
| **Open Security Groups** | Cloud Security | AWS / Cloud IAM | [Access Lab](https://learn.secbyte.org/ctf/open-security-groups-exposed-cloud-access-control) |
| **Cloud Secret Leakage** | Cloud Security | Cloud Configs | [Access Lab](https://learn.secbyte.org/ctf/cloud-secret-leakage-finding-hidden-credentials-in-cloud-con) |

---

## Categories

### Active Directory & Kerberos Attacks
Hands-on CTF labs covering Kerberos ticket extraction and offline password cracking techniques:

* **AS-REP Roasting:** Exploiting user accounts with Kerberos pre-authentication disabled to capture AS-REP responses for offline cracking.
  * Lab Link: https://learn.secbyte.org/ctf/as-rep-roasting-kerberos-preauth-abuse-detection
* **Kerberoasting:** Requesting TGS service tickets for accounts with Service Principal Names (SPNs) and extracting ticket hashes.
  * Lab Link: https://learn.secbyte.org/ctf/kerberoasting-from-kerberos-basics-to-ticket-abuse-detection

### Container Security & Docker Breakouts
Practical security labs analyzing container isolation mechanisms, namespace sharing, socket mounting, and host privilege escalation:

* **Container Secrets Exposure:** Identifying hardcoded secrets, environment variables, and build history leaks.
  * Lab Link: https://learn.secbyte.org/ctf/container-secrets-exposure
* **Root Containers Risk Analysis:** Risks associated with running container processes as UID 0 without user namespace remapping.
  * Lab Link: https://learn.secbyte.org/ctf/root-containers
* **Host Namespace Escape:** Exploiting shared host PID, network, or IPC namespaces to break out of container boundaries.
  * Lab Link: https://learn.secbyte.org/ctf/host-namespace-escape
* **Linux Container Breakout:** Techniques for breaking out of restricted container environments onto the underlying host system.
  * Lab Link: https://learn.secbyte.org/ctf/container-escape-linux-container-breakout
* **Mounted Docker Socket Control:** Exploiting exposed `/var/run/docker.sock` mounts to spawn privileged containers and obtain host root control.
  * Lab Link: https://learn.secbyte.org/ctf/mounted-docker-socket-container-breakout-to-host-control
* **Privileged Containers Misconfiguration:** Abusing `--privileged` flags and excessive kernel capabilities (`CAP_SYS_ADMIN`).
  * Lab Link: https://learn.secbyte.org/ctf/privileged-containers-from-misconfiguration-to-detection
* **Docker Escape to Host:** Escalating privileges from container scope to host file system access.
  * Lab Link: https://learn.secbyte.org/ctf/docker-escape-from-container-to-host-2

### Kubernetes & Cloud Infrastructure Security
Labs focusing on cloud access control misconfigurations, leaky repositories, and Kubernetes cluster escalation paths:

* **Kubernetes Misconfigurations:** Escalating privileges from a compromised Pod to full Kubernetes cluster takeover.
  * Lab Link: https://learn.secbyte.org/ctf/kubernetes-misconfigurations-from-pod-to-cluster-compromise
* **Open Security Groups:** Auditing and exploiting misconfigured cloud firewall rules and exposed access control lists.
  * Lab Link: https://learn.secbyte.org/ctf/open-security-groups-exposed-cloud-access-control
* **Cloud Secret Leakage:** Uncovering API keys, access tokens, and cloud credentials exposed in code bases and public storage.
  * Lab Link: https://learn.secbyte.org/ctf/cloud-secret-leakage-finding-hidden-credentials-in-cloud-con

---

## Learning Path

Follow this structured learning path to master cloud-native and container security:

1. **Active Directory Kerberos Foundations**
   - Practice AS-REP Roasting and Kerberoasting to understand offline password cracking dynamics.
2. **Container Fundamentals & Hardening**
   - Learn secret detection in images and analyze root container risks.
3. **Container Breakout & Host Escalation**
   - Practice host namespace escapes, Docker socket mounting abuse, and privileged container breakouts.
4. **Cloud & Cluster Security**
   - Audit Kubernetes RBAC and pod security policies.
   - Investigate exposed cloud security groups and credential leaks.

---

## How to Use the Labs

1. Choose a lab topic from the index table or category sections above.
2. Launch the interactive practice environment directly on Learn SecByte.
3. Complete the hands-on objectives covering enumeration, exploitation, and post-exploitation.
4. Review detection logs and mitigation guidelines to understand defensive hardening strategies.

---

## Disclaimer

This repository is strictly intended for educational, research, and defensive security purposes. All lab environments and concepts are provided to help cybersecurity students and practitioners identify vulnerabilities and harden modern infrastructure. Unauthorized testing against systems or networks without explicit permission is illegal.
