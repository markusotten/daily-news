# Citrix Product Updates — 2026-06-25

> Updates from the last 24 hours (June 24–25, 2026) across docs.citrix.com, docs.netscaler.com, and docs.xenserver.com.

---

## Citrix

### Citrix Workspace App for Mac — 2603.11

**Released:** June 24, 2026 | [Source](https://docs.citrix.com/en-us/citrix-workspace-app-for-mac/whats-new.html)

- Support for Citrix Snipping Tool integration (Technical Preview)
- DTLS 1.0 deprecated; application now defaults to DTLS 1.2 encryption
- Fixed: Connection failures when launching apps/desktops with SecureICA encryption enabled
- Fixed: Automatic launch issues after macOS 26.4 upgrades when using Workspace Launcher
- Fixed: Unexpected session disconnections over TCP caused by decryption failures
- Fixed: Session drops following network interruptions

---

### Citrix Workspace App for Linux — 2604

**Released:** June 25, 2026 | [Source](https://docs.citrix.com/en-us/citrix-workspace-app-for-linux/whats-new.html)

- Enhanced Browser Content Redirection with server-side certificate validation
- Entra ID single sign-on support for NetScaler Gateway stores
- Citrix Enterprise Browser removed from the package
- Google Chrome support for FIDO2 authentication
- Enhanced call connection times with UCSDK optimization
- Service continuity for connectorless workloads
- Shortcuts menu for macOS VDA
- Scanner workflow optimization through SANE caching
- EDT Lossy support with Secure HDX 2.0
- ARM64 support removed

---

### Citrix Endpoint Management — 26.5.0

**Documentation updated:** June 24, 2026 | [Source](https://docs.citrix.com/en-us/citrix-endpoint-management/whats-new)

- Android Credential Manager Support: new policy setting to control credential provider apps on Android Enterprise devices (requires Android 14+ and Secure Hub 26.5.0+)
- Android 17 compatibility for Android Enterprise devices
- Fixed: Manually editing Out of Compliance status not triggering Azure AD compliance status sync [XMHELP-4864]
- Fixed: iOS app updates via REST API failing with error 1493 [XMHELP-4898]
- Fixed: Public REST API authentication issues following migration [XMHELP-4903]

---

## XenServer

### XenServer 8.4 — Normal Channel Update

**Released:** June 24, 2026 | [Source](https://docs.xenserver.com/en-us/xenserver/8/whats-new/normal.html)

- New: Server-side API/CLI functionality to update existing VM Secure Boot certificates
- Improvement: AMD microcode updated to the 2026-05-19 release
- Fixed: Storage operations on remote hosts failing irreversibly in rare cases
- Fixed: Temporary configuration keys persisting on virtual disks after host crashes
- Fixed: Livepatches incorrectly applied when mandatory host reboots were required
- Fixed: License server unresponsiveness causing indefinite blocking during edition operations
- Fixed: Multi-part toolstack tasks timing out prematurely due to incorrect expiry calculations
