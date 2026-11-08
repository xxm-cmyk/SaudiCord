# SaudiCord security principles

## Account credentials
- Do not create a SaudiCord password form.
- Use Discord's supported sign-in flow; do not collect Discord passwords.
- Never print, display, transmit to a SaudiCord-operated service, or place account tokens in logs.
- Treat local session data as sensitive and follow Electron/Chromium secure storage practices.

## Plugins
- Treat every plugin as untrusted code until reviewed.
- Do not auto-enable newly installed plugins.
- Show source, version, requested capabilities, and scan results before approval.
- Use multiple scanners where available, but do not treat a clean scan as proof of safety.
- Prefer isolated execution and least privilege; plugins requiring broad access need explicit warnings and approval.
- Keep a review record and support rejection and revocation.

## Updates
- Accept updates only from the configured release source.
- Verify signed update metadata and artifact integrity before installation.
- Fail closed when signature or integrity verification fails.
- Keep a recoverable previous version where the updater supports it.

## Electron
- Keep context isolation enabled and Node integration disabled in renderer contexts.
- Validate IPC sender and payloads.
- Restrict navigation, permissions, and external protocol handling.
- Avoid remote code execution and unreviewed remote scripts.

## Scope
These are design requirements, not a claim that SaudiCord is already secure. Each control must be implemented and tested before release.
