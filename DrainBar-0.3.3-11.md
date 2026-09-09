# DrainBar 0.3.3

Claude credential access is more resilient.

- Background checks, startup, and wake no longer display Keychain password prompts. Choose Refresh when access needs approval.
- A still-valid Claude credential stays in memory during temporary Keychain access problems. No extra token copy is saved to disk.
- DrainBar detects replacement credentials and retries once with a newer token before reporting an expired sign-in.
- Removed credentials and explicit Keychain denial clear the retained credential.

Claude Code continues to manage sign-in and token renewal.
