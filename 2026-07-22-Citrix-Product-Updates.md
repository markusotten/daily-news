# Citrix Product Updates — 2026-07-22

Summary of "What's New" documentation updates published in the last 24 hours (2026-07-21 to 2026-07-22) across [docs.citrix.com](https://docs.citrix.com), [docs.netscaler.com](https://docs.netscaler.com), and [docs.xenserver.com](https://docs.xenserver.com).

## Citrix

### Workspace Environment Management (service)

Source: [Workspace Environment Management (service) What's New](https://docs.citrix.com/en-us/workspace-environment-management/service/whats-new.html)

- Administrative logging — track all configuration changes made by administrators in the WEM web console; each log entry captures the admin identity, affected object, operation type, and a before/after change summary, retained for 180 days (max 100,000 records), with WEM Full admins seeing all logs and WEM Restricted admins seeing only logs scoped to their assigned configuration sets.
- Modeling wizard — select a user to instantly see all WEM actions and security assigned to them, organized by action type, along with the user's group membership and OU placement.
- Summary view added to the Reports page, with four charts: Event type, Action processing results, Configuration set, and Script execution results.
- Enhancements to the Profile tab in Agent Insights — now supports a broader range of user profile types beyond profile containers, and shows real-time scan progress with an estimated time remaining during profile data refresh.
- New built-in scripts for AOT diagnostics and log collection — five new built-in scripts added: Diagnose Citrix AOT issues, Collect Citrix diagnostic logs, Collect Windows Event Logs, and Collect Citrix Scout diagnostics.
- Fix: the WEM Agent might consume excessive resources during session launch when the Logoff External Task trigger is enabled and many GPOs are configured. [WEM-51116]

## NetScaler

No updates in the last 24 hours.

## XenServer

No updates in the last 24 hours.
