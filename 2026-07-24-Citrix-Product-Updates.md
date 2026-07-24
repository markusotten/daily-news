# Citrix Product Updates — 2026-07-24

Summary of "What's New" documentation updates published in the last 24 hours (2026-07-23 to 2026-07-24) across [docs.citrix.com](https://docs.citrix.com), [docs.netscaler.com](https://docs.netscaler.com), and [docs.xenserver.com](https://docs.xenserver.com).

## Citrix

### StoreFront 2603 (Current Release)

Source: [StoreFront What's New](https://docs.citrix.com/en-us/storefront/current-release/whats-new.html)

- System requirement: StoreFront now requires .NET 10 (automatically installed if absent).
- Entra ID Identity Support (Preview): now configurable via the management console (previously PowerShell-only); adds Citrix Virtual Apps and Desktops site inclusion for hybrid identities, FAS enablement for hybrid-identity users on AD/hybrid-joined VDAs, and reduced memory usage for large Entra group memberships.
- Entra ID SSO to VDAs (Preview): management console configuration; combined Entra ID + FAS SSO support based on delivery group logon type; support for Citrix Virtual Apps and Desktops 2603+ with hybrid-joined VDAs.
- Launch Telemetry: ICA files now include a "[Session Launch Telemetry]" section with process stage timestamps (excluded when ICA signing is enabled).
- Windows Server Core support: installation without desktop experience using the `-silent` flag, with PowerShell-only management (no console access).
- Now includes Citrix Workspace app for HTML5 HDX client 2603.
- 14 documented issues fixed, including authentication reset problems, localization issues, Activity Manager reconnection failures, header deprecation, branding color defaults, and console functionality problems.

## XenServer

### XenServer 9 (Normal channel)

Source: [XenServer 9 What's New (Normal channel)](https://docs.xenserver.com/en-us/xenserver/9/whats-new/normal)

- Improvement: Updated OpenSSL to v3.5.7.
- Improvement: Updated broadcom-bnxt-en driver to 1.10.3_239.1.68.0.
- Improvement: Updated broadcom-mpi3mr driver to 8.17.1.0.0.
- Improvement: Updated intel-ice driver to v2.6.4.
- Improvement: Updated avago-megaraid-sas driver to 07.737.03.00.
- Improvement: Enhanced control plane performance with large numbers of active VDIs.
- Fixed: A rare core dump could occur during VM shutdown on GFS2 or XFS storage.
- Fixed: Storage lifecycle operations could be delayed when a file-based SR is unreachable.
- Fixed: Potential data corruption on SMB3 SR with multi-host access.
- Fixed: A resource leak could occur during license application.
- Fixed: BIOS-boot PVS virtual machines could fail DHCP lease acquisition.
- Security: Resolved 19 CVEs, including CVE-2026-42767, CVE-2026-45447, CVE-2026-45446, CVE-2026-45445, CVE-2026-42770, CVE-2026-42769, CVE-2026-42768, CVE-2026-42766, CVE-2026-42764, CVE-2026-34183, CVE-2026-34182, CVE-2026-34181, CVE-2026-34180, CVE-2026-9076, CVE-2026-7383, CVE-2026-31790, CVE-2026-31789, CVE-2026-28388, CVE-2026-28390, and CVE-2026-28389.
