# DrainBar 0.3.4

Claude credential access is more resilient, with an updated secure installer.

- Background checks, startup, and wake no longer display Keychain password prompts. Choose Refresh when access needs approval.
- A still-valid Claude credential stays in memory during temporary Keychain access problems. No extra token copy is saved to disk.
- DrainBar detects replacement credentials and retries once with a newer token before reporting an expired sign-in.
- Removed credentials and explicit Keychain denial clear the retained credential.
- Updated Sparkle to 2.9.6, including upstream installer security fixes.

Claude Code continues to manage sign-in and token renewal.
