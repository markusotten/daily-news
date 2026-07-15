# Citrix Product Updates — 2026-07-15

Summary of "What's New" documentation updates published in the last 24 hours (2026-07-14 to 2026-07-15) across [docs.citrix.com](https://docs.citrix.com), [docs.netscaler.com](https://docs.netscaler.com), and [docs.xenserver.com](https://docs.xenserver.com).

## Citrix

No updates in the last 24 hours.

## NetScaler

### NetScaler Console service

Source: [NetScaler Console service What's New](https://docs.netscaler.com/en-us/netscaler-console-service/release-notes/whats-new.html)

- Added unified GeoIP database synchronization across Console, agents, and managed instances, with Sync Now/scheduled sync options, history logs, and a sync status panel.
- Added telemetry diagnostics covering device and agent status, error codes, and live connectivity checks.
- Fixed: analytics data missing after a cloud migration.
- Fixed: false-positive Config Audit alerts related to LAS.
- Fixed: missing source IPs in cloud agent logs.
- Fixed: SSL certificate download returning 404 errors.
- Fixed: "invalid resource" error when editing user groups.

## XenServer

### XenCenter

Source: [XenCenter What's New](https://docs.xenserver.com/en-us/xencenter/current-release/whats-new.html)

- Released XenCenter 2026.4.0, which includes a security fix documented in [Security Bulletin CTX696811](https://support.citrix.com/support-home/kbsearch/index?articleId=CTX696811).
- Documented known issue: the host General tab does not refresh immediately after a host reboot.
- Documented known issue: a font/DPI scaling display issue.
- Documented known issue: the MAC address is preserved on VM export/import, risking IP conflicts.
- Documented known issue: OVF/disk-image import fails when the folder name contains "#".
- Documented known issue: a XenCenter CLI argument-quoting issue.
- Documented known issue: OVF signature verification failure.
- Documented known issue: the Import Wizard crashes when a running import is cancelled.
