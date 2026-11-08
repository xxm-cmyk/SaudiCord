# SaudiCord 🇸🇦

**Discord, لكن بتجربة عربية أفضل.**

SaudiCord is an independent, Arabic-first desktop client project based on the open-source Vesktop project. It aims to preserve Discord's familiar interface while improving Arabic localization, right-to-left layout, plugin management, security review, and update reliability.

> SaudiCord is not a separate chat network or account system. Discord remains the service provider for accounts, messages, servers, and voice.

## Project goals

- Full Arabic interface and correct RTL behavior without redesigning Discord's familiar UI.
- Windows 10/11 support as the initial release target.
- In-app plugin creation and management, with explicit review and approval before distribution.
- Safer plugin handling: source review, automated scanning, permission review, and clear warnings. Automated scanners cannot guarantee that code is safe.
- Reliable automatic updates with integrity verification and signed releases.
- Never collect Discord passwords or expose account tokens through an owner dashboard.

## Upstream

The desktop foundation is [Vesktop](https://github.com/Vencord/Vesktop), which is licensed under **GPL-3.0-or-later**. SaudiCord must preserve applicable license notices and provide corresponding source for distributed derivative builds.

## Development status

Early setup. The repository currently contains project documentation; the Vesktop source tree has not yet been imported. No installable build is available yet.

## Planned milestones

1. Import and pin a reviewed Vesktop upstream revision while preserving license files and notices.
2. Rename application identity and Windows packaging metadata to SaudiCord.
3. Implement Arabic localization and RTL, then test mixed Arabic/English text and core Discord flows.
4. Design a restricted plugin workflow with staged review and explicit owner approval.
5. Harden Electron boundaries and establish signed, verifiable automatic updates.
6. Add Windows build and regression tests.

## License

The project is intended to remain compatible with the upstream GPL-3.0-or-later codebase. See the upstream license and retain all required notices when importing its source.
