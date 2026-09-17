# DrainBar 0.3.9

- Fixes repeated Claude Keychain password prompts caused by automatic sign-in renewal.
- Uses the same Apple credential access path as Claude Code and verifies renewed credentials after saving.
- Checks existing Keychain permissions before background access and stops repeated attempts after an access failure or timeout.
