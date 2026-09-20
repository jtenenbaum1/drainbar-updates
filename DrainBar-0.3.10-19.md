# DrainBar 0.3.10

- Adds a one-time in-app Claude sign-in stored privately in macOS Keychain, keeping usage current without rewriting Claude Code credentials.
- Keeps the Claude session and supporting web cookies current while preventing scheduled refreshes from opening Keychain password prompts.
- Corrects oversized credential failures so they are no longer presented as Keychain permission problems.
