# Citrix Product Updates — 2026-07-23

Updates published in the "What's New" / release notes sections in the last 24 hours across [docs.citrix.com](https://docs.citrix.com), [docs.netscaler.com](https://docs.netscaler.com), and [docs.xenserver.com](https://docs.xenserver.com).

## Citrix

### Citrix Workspace app for HTML5

Source: [What's new in 2603.10](https://docs.citrix.com/en-us/citrix-workspace-app-for-html5/whats-new.html)

- This release addresses areas that improve overall performance and stability.
- Fixed: When you start a resource from DaaS using Citrix Workspace app for HTML5, the session might fail on the first attempt if the target VDA is powered off and takes more than three minutes to start and register, though the subsequent attempt succeeds. [CCVADHELP-5191]
- Fixed: When you try to create a file using the Windows Save dialog on a drive that Client Drive Mapping (CDM) maps in a Citrix Workspace app for HTML5 session, the file creation might fail. [CVADHELP-32584]
- Fixed: During a desktop session, the mouse cursor might intermittently stop responding, failing to update its shape (e.g., remains an arrow instead of changing to a text cursor). [CVADHELP-33365]
- Fixed: The Auto-fit Screen (Fit_To_Window) setting, configured through Global App Configuration Service (GACS), might not persist when a session reconnects, causing sessions to reset to default Device Pixel Ratio (DPR) mode. [CVADHELP-33365]
- Fixed: When using Client Drive Mapping (CDM) to map files or folders within Citrix Workspace app for HTML5, some files might be missing in the mapped network drive. [CVADHELP-33220]
- Fixed: You can't paste content between your local endpoint and a Citrix Workspace app for HTML5 session through the Clipboard Toolbar unless you manually click the clipboard dialog. [CVADHELP-33180]

### Citrix Secure Access for iOS

Source: [Release Notes — V26.06.1](https://docs.citrix.com/en-us/citrix-secure-access/citrix-sso-release-notes-ios.html)

- Fixed: Users might experience a failure to re-establish the connection when switching networks. [NSHELP-44311]
