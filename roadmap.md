---
description: View future plans and current status
---

# Roadmap

#### Phase 1: Core Infrastructure & Networking

_Goal: Establish a secure perimeter and centralize network identity and addressing._

* [x] Physical Host Deployment: Configure HP EliteDesk 705 with Proxmox VE.
* [ ] Perimeter Security: Finalize OPNsense firewall rules and isolation for the WAN/Security zone.
* [ ] Identity Services (DC01): Promote Windows Server 2022 to Domain Controller and install AD DS.
* [ ] Core Networking: Configure Enterprise DNS and DHCP scopes on the primary Domain Controller.

#### Phase 2: High Availability & Web Services

_Goal: Implement redundancy and internal service hosting._

* [ ] Service Redundancy (DC02): Deploy a secondary Domain Controller to manage replication and failover.
* [ ] Web Infrastructure: Deploy Windows Server 2022 running IIS to host internal organizational resources.
* [ ] Connectivity Testing: Verify cross-zone communication and service availability from the trusted LAN.

#### Phase 3: Fleet Management & Scalability

_Goal: Standardize end-user environments and streamline deployment._

* [ ] Golden Image Creation: Build a "master" Windows Client image, fully patched and sysprep-ready.
* [ ] Template Conversion: Convert the master image to a Proxmox template for rapid scaling.
* [ ] Fleet Deployment: Deploy linked clones for Client-01 and Client-02 and perform automated domain joins.

#### Phase 4: Governance & Security Operations

_Goal: Implement administrative controls and offensive security testing._

* [ ] Identity Population: Build an OU structure reflecting a corporate hierarchy with test users and groups.
* [ ] Policy Management: Design and deploy Group Policy Objects (GPOs) for environment hardening (MFA, restricted control panel, etc.).
* [ ] Offensive Audit: Utilize the Kali Linux VM in the Red Zone to perform vulnerability scans and test firewall egress/ingress rules.
* [ ] Cloud Integration: Establish a sync between on-premise Active Directory and Microsoft Entra ID.
