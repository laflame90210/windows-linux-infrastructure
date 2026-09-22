# Windows Server & Linux Infrastructure

**Windows Server 2022 · CentOS · Active Directory · Infrastructure Services**

## Overview

An academic infrastructure lab completed in Winter 2026, combining Windows Server and Linux services across three network segments. The project brings together identity management, network services, web hosting, file sharing, remote access, and messaging.

**Status:** Completed academic project, documented in the final Windows Server and Linux report.

## Infrastructure

| Area | Implementation documented |
| --- | --- |
| Identity | Parent and child Active Directory domains, OUs, users, and administrative groups |
| Policy | GPOs for application restrictions, software deployment, logon messaging, and printer deployment |
| Addressing and routing | Static server interfaces, RRAS with RIP v2, DHCP scopes, and DHCP relay |
| Storage | NTFS data volume and a hard quota managed with FSRM |
| Windows web services | Multiple IIS sites using host headers, plus FTP |
| Deployment | WDS boot and Windows 10 Enterprise installation images |
| Linux services | BIND DNS, NFS, Samba, Apache, and CUPS printing |
| Remote access | VPN connectivity with NPS/RADIUS integration |
| Messaging | Exchange mailboxes and internal email delivery |

## Work and validation

- Built the parent/child domain structure and organized departmental OUs and accounts.
- Linked and tested Group Policy settings and shared printer deployment.
- Configured DHCP for all three segments, including clients reached through a relay.
- Hosted and accessed IIS websites and tested FTP connectivity.
- Prepared WDS images for operating system deployment.
- Configured Linux file and printing services accessible from Windows clients.
- Established a VPN client connection and checked its assigned IP and DNS settings.
- Tested Exchange email delivery between domain users through Outlook Web Access.

## Troubleshooting documented

| Issue | Investigation focus |
| --- | --- |
| Remote clients did not receive DHCP leases | Relay configuration and matching DHCP scopes |
| DNS failures following child domain setup | Domain DNS configuration and replication checks |
| GPOs did not apply as expected | Policy scope, refresh, and resultant policy checks |
| VPN connection failed | NPS policy and authentication logs |
| Exchange browser certificate warning | Certificate configuration and the client access name |

## What I learned

This project connected individual server roles into one working environment. It strengthened my understanding of how DNS, authentication, routing, policy, and client configuration depend on one another, and the importance of checking each layer when troubleshooting.

## Documentation scope

This repository summarizes the completed lab report. The lab includes course-specific settings and legacy services; its configurations describe an educational environment rather than a production deployment template. Original VM images and full configuration exports are not included here.

The standalone [Exchange lab](https://github.com/laflame90210/exchange-server-lab) provide related portfolio entries.


---
[Back to my portfolio](https://github.com/laflame90210)
