# DrainBar 0.3.1

Service health is now visible at a glance for Claude and OpenAI.

- New green, yellow, and red status indicators appear beside each provider's
  latest usage timestamp.
- Click a status indicator to open that provider's official service-status
  page.
- Claude and Codex menu-bar marks turn yellow for degraded service and red for
  an outage. Healthy and unavailable states keep the normal menu-bar color.
- Service health refreshes at launch, when the popover opens, with manual
  refreshes, and periodically in the background.
- VoiceOver labels and tooltips announce degraded and outage states without
  relying on color alone.
