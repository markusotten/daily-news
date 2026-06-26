# Citrix Product Updates — 2026-06-26

*Automated daily digest of What's New documentation updates from docs.citrix.com, docs.netscaler.com, and docs.xenserver.com.*

> No documentation updates were published in the strict last-24-hour window (June 25–26, 2026). The entries below reflect the most recently published changes in each product's What's New section.

---

## Citrix (docs.citrix.com)

### Citrix Endpoint Management
**Updated: June 24, 2026** | [What's New](https://docs.citrix.com/en-us/citrix-endpoint-management/whats-new.html)

- **Credential Manager Support on Android** *(v26.5.0)* — New Restrictions policy option permits apps to function as credential providers on Android 14 and later.
- **Android 17 Compatibility** *(v26.5.0)* — Android Enterprise devices running the latest Android 17 OS are now officially supported.

### Citrix Workspace App
**Updated: June 24, 2026** | [What's New](https://docs.citrix.com/en-us/citrix-workspace-app/whats-new)

- **Mac 2603.11 — Citrix Snipping Tool Integration (Technical Preview)** — Citrix Snipping Tool integration is now available as a Technical Preview on macOS.
- **Mac 2603.11 — Deprecation of DTLS 1.0** — Datagram Transport Layer Security (DTLS) 1.0 is deprecated in Citrix Workspace App for Mac.
- **Windows 2603.10 — Cisco Webex VDI Plugin Support for 64-bit** *(June 19, 2026)* — The 64-bit Cisco Webex VDI plugin is now available via manual installation or using the silent deployment parameter `CitrixWorkspaceapp.exe ADDONS=WebexVDIPlugin`. ([What's New – Windows](https://docs.citrix.com/en-us/citrix-workspace-app-for-windows/whats-new))

### Citrix DaaS Flex
**Updated: June 23, 2026** | [What's New](https://docs.citrix.com/en-us/citrix-daas-flex/azure/whats-new.html)

- **Microsoft Entra ID and Intune Support** — Citrix DaaS Flex now integrates with Microsoft Entra ID and Intune to strengthen security and compliance; pairs with Microsoft Entra single sign-on for simplified user access.
- **Manage IPv4 Address Ranges for Azure Virtual WAN** — Administrators can now expand network capacity by adding IPv4 address ranges to Citrix-managed spoke virtual networks after initial setup.

### Citrix DaaS
**Updated: June 17, 2026** | [What's New](https://docs.citrix.com/en-us/citrix-daas/whats-new.html)

- **Access Citrix DaaS Data in Aidrien** — Aidrien can retrieve environment data (machines, sessions, machine catalogs, delivery groups) directly in chat for investigation without leaving the conversation.
- **App Protection Reporting in Citrix Monitor** — Real-time reporting of protection policy activations and security risk detections is now available in Citrix Director and Monitor for proactive risk management.
- **Azure SSD Storage Types for Ephemeral OS Disks** — Studio now allows selection of base OS managed disk storage types (Premium SSD, Standard SSD, Standard HDD) for Azure Ephemeral OS Disks during catalog creation.
- **Endpoint OS Version Visibility** — Session and Connection pages now include an Endpoint OS Version column and filter for Windows and Linux device management.
- **Improved Bulk Actions in Web Studio** — All matching items across multiple pages can now be selected at once, removing the previous 500-item bulk operation limit.

### Citrix Secure Web
**Updated: June 4, 2026** | [What's New](https://docs.citrix.com/en-us/citrix-secure-web/whats-new.html)

- **Secure Web for iOS 26.5.0** — Performance and stability improvements.
- **Secure Web for Android 26.2.0** — Added 16 KB memory page size support to optimize performance and comply with Google Play requirements.

---

## NetScaler (docs.netscaler.com)

### NetScaler Console Service
**Updated: June 17, 2026** | [What's New](https://docs.netscaler.com/en-us/netscaler-console-service/release-notes/whats-new)

- **Analytics — BOT Violation Processing Fix** — Resolved issues with BOT violation data processing in the Analytics module.
- **Infrastructure — Instance Visibility Controls** — Fixed instance visibility control issues in the Infrastructure module.
- **Security — WAF Recommendation Application Fix** — Resolved errors when applying WAF (Web Application Firewall) recommendations.
- **Certificate Management Improvements** — Multiple fixes and improvements to the certificate management workflows.

---

## XenServer (docs.xenserver.com)

### XenServer 8.4
**Updated: June 9, 2026** | [What's New](https://docs.xenserver.com/en-us/xenserver/8/whats-new)

- **Windows 11 and vTPM Support** — VMs can now leverage a virtual TPM 2.0-compliant API, enabling Windows 11 compatibility.
- **License Activation Service (LAS)** — File-based licensing reached end-of-life on April 15, 2026; all deployments now use the License Activation Service.
- **VM Customization via Sysprep** — Running Windows VMs can now be programmatically customized by passing a Sysprep answer file.
- **Local XFS Storage Repository** — New local XFS storage type added; changed block tracking expanded to GFS2 and XFS SR types.
- **Third-Party Monitoring via NRPE and SNMP** — New integration support for NRPE and SNMP enables third-party monitoring tools.
- **Certificate Verification Enabled by Default** — Fresh installations now have certificate verification enabled; option available to restrict TCP port 80 usage.

### XenServer 9 Preview
**Updated: June 3, 2026** | [What's New](https://docs.xenserver.com/en-us/xenserver/9/whats-new)

- **NUMA Optimization** — Improved VM performance on multi-socket systems through enhanced NUMA affinity.
- **Host Secure Boot (Preview)** — Secure Boot support for XenServer hosts is available in preview.
- **Driver Multi-version Management** — Multiple driver versions can now be managed simultaneously on a single host.
- **Xen Hypervisor v4.21** — Updated to the latest Xen hypervisor release.
- **Dom0 Kernel Upgraded to v6.x** — The control domain (dom0) kernel has been updated to version 6.x.
- **GFS2 SRs Migrated to Corosync3** — Cluster file system storage repositories updated to use Corosync3.
- **HTTP Port 80 Disabled by Default** — TCP port 80 is now disabled by default on new installations for improved security.
- **Dropped Support for SUSE Linux Enterprise Desktop 12 SP4** — Legacy guest OS support removed.
