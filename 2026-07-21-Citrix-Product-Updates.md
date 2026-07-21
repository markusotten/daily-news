# Citrix Product Updates — 2026-07-21

Summary of "What's New" documentation updates published in the last 24 hours (2026-07-20 to 2026-07-21) across [docs.citrix.com](https://docs.citrix.com), [docs.netscaler.com](https://docs.netscaler.com), and [docs.xenserver.com](https://docs.xenserver.com).

## XenServer

### XenServer 9 (Early Access channel)

Source: [XenServer 9 What's New — Early Access channel](https://docs.xenserver.com/en-us/xenserver/9/whats-new/early-access)

- Updated OpenSSL to v3.5.7.
- Updated broadcom-bnxt-en driver to 1.10.3_239.1.68.0.
- Updated broadcom-mpi3mr driver to 8.17.1.0.0.
- Updated intel-ice driver to v2.6.4.
- Updated avago-megaraid-sas driver to 07.737.03.00.
- Enhanced control plane performance when numerous VDIs are active on individual hosts.
- Fixed: a rare core dump could occur during VM shutdown when using GFS2 or XFS storage repositories.
- Fixed: storage lifecycle operations could be delayed when a file-based SR is unreachable, even for unrelated operations.
- Fixed: potential data corruption on SMB3 SR accessed from multiple hosts.
- Fixed: a resource leak could occur during license application.
- Fixed: BIOS-boot PVS virtual machines could fail to obtain a DHCP lease.
- Security: addressed 19 CVEs, including CVE-2026-42767, CVE-2026-45447, CVE-2026-45446, CVE-2026-45445, CVE-2026-42770, CVE-2026-42769, CVE-2026-42768, CVE-2026-42766, CVE-2026-42764, CVE-2026-34183, CVE-2026-34182, CVE-2026-34181, CVE-2026-34180, CVE-2026-9076, CVE-2026-7383, CVE-2026-31790, CVE-2026-31789, CVE-2026-28388, CVE-2026-28390, and CVE-2026-28389.

### XenServer 8.4 (Early Access channel)

Source: [XenServer 8.4 What's New — Early Access channel](https://docs.xenserver.com/en-us/xenserver/8/whats-new/early-access.html)

- Updated OpenSSL to v3.5.7.
- Fixed: storage lifecycle operations could be delayed when a file-based SR is unreachable, even if the operation did not directly involve the affected SR.
- Fixed: specific firmware could place MMCFG regions in an E820 memory hole, making them inaccessible to the hypervisor and preventing use of SR-IOV devices in VMs.
- Fixed: Xen could fail to boot on certain systems due to an issue with merged PDX ranges.
- Fixed: Xen could fail to boot on certain systems due to an issue with non-aligned memory affinity ranges.
- Security: included 19 upstream code changes addressing CVEs spanning CVE-2026-42767 through CVE-2026-28389.

## Citrix

No updates in the last 24 hours.

## NetScaler

No updates in the last 24 hours.
