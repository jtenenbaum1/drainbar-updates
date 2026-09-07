# DrainBar 0.3.0

A safety and clarity release. DrainBar now only ever reads from the tools it
watches, explains itself in plain language, and is easier to set up.

## Please note

**DrainBar no longer refreshes your Claude sign-in.** Earlier versions wrote a
renewed token back into Claude Code's own credential store. DrainBar now only
reads. When the sign-in expires, DrainBar keeps showing your last usage, marks
it stale, and asks you to run `claude` in Terminal so Claude Code renews its own
sign-in. Nothing else changes about how usage is read.

**Codex now defaults to Live account usage.** New installs read current limits
straight from your account. If you previously chose Local session files, your
choice is kept.

## Setup and first run

- A short welcome window on first launch shows which tools were found, explains
  exactly what DrainBar reads, and lets you turn on notifications and Launch at
  Login.
- Changing accounts now shows the exact Terminal commands with a Copy button,
  instead of opening a Terminal window and running commands for you.
- Notifications are requested when you ask for them, not silently at launch.

## Clearer in daily use

- Errors are written in plain language. "Sign-in expired" and "Keychain access
  needed" replace raw status codes and internal messages.
- A denied Keychain prompt no longer repeats on every refresh.
- Larger, more legible text in the popover, with VoiceOver labels on the menu
  bar meter and each usage row.
- The menu bar item has a tooltip describing the focused window.
- Refresh shows progress instead of appearing to do nothing.
- Standard menu with About, Settings, Welcome and Quit, so Command Q and
  Command W behave as expected.

## Appearance

- The ring style no longer repeats the provider logo beside the ring. The logo
  sits in the middle, larger and clear of the ring, and the readout is narrower.
- New "Show sample data" option under Settings, General fills the meters with
  example usage. Useful for trying DrainBar before signing in.

## Under the hood

- Both providers share one hardened network path: no cookies, no stored
  credentials, no redirects, and a request timeout.
- DrainBar never writes to another tool's credential store.
