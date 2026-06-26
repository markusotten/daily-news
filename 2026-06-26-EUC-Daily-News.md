# EUC Daily News — June 26, 2026

*Daily digest of Citrix/NetScaler and wider EUC news. Window: June 25–26, 2026.*

---

## Security Advisories

### CVE-2026-3055 "CitrixBleed 3" — Large-Scale Exploitation Wave Confirmed in June

**Severity:** Critical (CVSS v4.0: 9.3) | **Patched:** March 23, 2026 | **Active exploitation:** June 2026

- Out-of-bounds memory read on NetScaler ADC/Gateway appliances configured as a **SAML Identity Provider**
- Unauthenticated attackers send crafted `SAMLRequest` payloads to `/saml/login` omitting the `AssertionConsumerServiceURL` field, triggering the appliance to leak kilobytes of process memory (session tokens, SAML assertions, credentials) via the `NSC_TASS` cookie
- Fortinet confirmed **large-scale exploitation** in early June — an 11-week gap between patch and active attack wave
- Security researchers are calling this **CitrixBleed 3** due to identical vulnerability class to the 2023 and 2025 predecessors
- **Critical:** Patching alone does not invalidate already-exfiltrated session tokens. All active sessions must be explicitly flushed after applying the fix

**Affected versions:**
| Build | Fixed in |
|---|---|
| NetScaler ADC/Gateway 14.1 | 14.1-66.59 and later |
| NetScaler ADC/Gateway 13.1 | 13.1-62.23 and later |
| NetScaler ADC 13.1-FIPS / 13.1-NDcPP | 13.1-37.262 and later |

**Sources:** [Official Bulletin CTX696300](https://support.citrix.com/external/article/CTX696300/netscaler-adc-and-netscaler-gateway-secu.html) | [ZeroHunt.ai analysis](https://zerohunt.ai/blog/citrixbleed-3-netscaler-cve-2026-3055/) | [The Hacker News](https://thehackernews.com/2026/03/citrix-urges-patching-critical.html)

---

### CVE-2026-4368 — Session Mixup on Gateway/AAA Virtual Servers

**Severity:** High (CVSS v4.0: 7.7) | **Patched:** March 23, 2026

- Race condition causes user session tokens to be mixed up between concurrent users on appliances configured as Gateway (SSL VPN, ICA Proxy, CVPN, RDP Proxy) or AAA virtual servers
- Affects only build **14.1-66.54**; fixed in 14.1-66.59 and later
- Disclosed in the same bulletin as CVE-2026-3055 (CTX696300)

**Source:** [Official Bulletin CTX696300](https://support.citrix.com/external/article/CTX696300/netscaler-adc-and-netscaler-gateway-secu.html)

---

### Citrix Validates June 2026 Microsoft Patches — Known Audio Issue with KB5094126

**Source:** [Citrix KB CTX696710](https://support.citrix.com/external/article/CTX696710/microsoft-security-update-validation-rep.html)

Citrix's June 2026 Microsoft Security Update Validation Report confirms Patch Tuesday updates pass testing across CVAD 2203 CU7, 2402 CU4, 2507 CU1, and 2603. One known issue:

- **KB5094126** on **Windows 11 24H2/25H2 multi-session VDAs** causes audio volume in Citrix ICA sessions to automatically reset to 0% and become non-adjustable; additional audio device malfunctions may occur
- Citrix recommends testing all June updates in a dev/staging environment before pushing to production

---

## Citrix

### Citrix Launches DaaS Flex — Credit-Based Virtual PC Delivery

**Published:** June 18, 2026 | [The Register](https://www.theregister.com/virtualization/2026/06/18/citrixs-daas-flex-aims-to-delay-pricey-pc-upgrades/5258476)

Citrix officially productized **Citrix DaaS Flex**, a credit-based virtual PC delivery model positioned as an alternative to costly hardware refresh cycles. Key details:

- Deployment starts with an endpoint fleet assessment that identifies underutilized machines and recommends one of three user *personas* (task worker, knowledge worker, power user)
- Delivery options: full cloud PCs on Microsoft Azure, managed browsers, or published applications
- Pricing uses a credit system on multi-year contracts (three-year minimum); Citrix absorbs costs when daily usage stays within the 10–14 hour operational window
- Pairs with Microsoft Entra ID and Intune for identity and compliance management

---

### Citrix and HPE Deepen Strategic Collaboration on Private Cloud and Virtualization

**Published:** June 17, 2026 | [BusinessWire](https://www.businesswire.com/news/home/20260617627634/en/Citrix-and-HPE-to-Deepen-Strategic-Collaboration-on-Private-Cloud-and-Virtualization-Solutions)

Citrix (Cloud Software Group) and HPE announced expanded joint engineering, product integration, and go-to-market plans targeting enterprises with strict data sovereignty and regulatory requirements:

- **HPE GreenLake** positioned as the premier infrastructure platform for Citrix Platform Flex on-premises and sovereign cloud workloads
- **Citrix DaaS and CVAD** to integrate with **HPE Morpheus Software** (VM Essentials virtualization) and **HPE CloudOps** for unified orchestration, automation, and observability
- Industry-specific solution offerings and joint sales channel enablement planned
- *"Modern desktop delivery that gives [customers] flexibility without requiring them to compromise on control or performance"* — Shawn Bass, Citrix SVP

---

## Competitors

### Microsoft AVD / Windows 365 — June 2026 Feature Wave

**Sources:** [AVD What's New](https://learn.microsoft.com/en-us/azure/virtual-desktop/whats-new) | [Partner Center June 2026](https://learn.microsoft.com/en-us/partner-center/announcements/2026-june) | [Windows 365 at Build 2026](https://techcommunity.microsoft.com/blog/windows-itpro-blog/made-for-developers-and-agents-windows-365-at-build-2026/4519041)

**Azure Virtual Desktop Hybrid — Public Preview**
AVD Hybrid extends Microsoft's cloud-managed control plane to on-premises infrastructure. Organizations run session hosts on their own hardware while Microsoft manages brokering, monitoring, and policy. Targets customers with data residency requirements or hybrid datacenter strategies.

**Windows Cloud Keyboard Input Protection — Preview**
Encrypts keystrokes at the kernel level on Windows 365 and AVD session hosts to block keylogger-class attacks. Purpose-built for BYOD and regulated-industry deployments where endpoint trust is limited.

**Context-Based Redirections — Public Preview**
Server-side capability dynamically controls clipboard, printer, drive, and USB redirection based on user identity, device compliance posture, and network conditions — removing reliance on client-side policy enforcement.

**RDP Multipath with Redundant TCP — Generally Available**
Maintains multiple transport paths (UDP + TCP) simultaneously between client and session host for improved connection resiliency and failover without session disruption.

**Windows 365 Frontline → Windows 365 Flex (Rebrand)**
Windows 365 Frontline has been renamed to Windows 365 Flex. No functional changes to the shared Cloud PC model; reflects updated market positioning.

**Windows 365 GPU Enterprise Select 256 GB — CSP Availability July 1**
This SKU was temporarily removed from the Cloud Solution Provider channel for system configuration updates; returns for CSP purchase on July 1, 2026.

**Azure Virtual Desktop Classic — New Tenant Creation Blocked**
AVD Classic now prevents creation of new tenants. Full retirement is scheduled for September 2026. Organizations still on Classic must migrate to Azure Virtual Desktop (ARM-based) before that date.

---

### Omnissa Workspace ONE ITSM Connector 9.0.0

**Published:** June 21, 2026 | [Releasebot.io](https://releasebot.io/updates/omnissa)

Omnissa released a significant update to the Workspace ONE ServiceNow connector:

- Organization group-based access controls for device remediation workflows
- Mobile DEX telemetry data surfaced directly within ServiceNow tickets
- Device search by friendly name
- Configurable tab visibility (UEM, Experience, Horizon) per admin role
- DEX history extended from 24 hours to **90 days**
- Certified for ServiceNow Australia release

---

## Community

### Nerdio: "How to Choose a Desktop Virtualization Model in 2026"

**Published:** June 25, 2026 | [Nerdio Blog](https://getnerdio.com/blog/desktop-virtualization/)

Nerdio published a comprehensive decision guide for IT leaders evaluating desktop virtualization in 2026. Key framing:

- Three urgent drivers pushing decisions now: Windows 10 end-of-life, legacy platform renewal (Citrix/Omnissa), and shifting hardware economics
- Recommends **workforce segmentation** rather than a single model: task workers on pooled multi-session VDAs, knowledge workers on fixed Cloud PCs, power users on GPU-accelerated VMs
- Compares on-premises VDI, RDS, Azure Virtual Desktop, and Windows 365 on cost, compliance posture, Teams multimedia support, and management overhead
- Cites examples of 14-day deployment timelines and meaningful cost reductions using managed DaaS with modern tooling
