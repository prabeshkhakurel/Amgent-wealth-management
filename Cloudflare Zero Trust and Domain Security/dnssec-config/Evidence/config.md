# DNSSEC Configuration

**Task:** Configure DNSSEC
**Jira Task:** KAN-26
**Status:** In Progress

## Findings

- Enabled DNSSEC on the Cloudflare side; Cloudflare generated a
  DS record for the domain
- Crazy Domains self-service dashboard (Name Servers, DNS
  Settings, Administration tabs) has no option to add a DS record
  — appears to require contacting Crazy Domains support directly
  for domains using an external DNS provider
- Logged as a blocker; next step is to raise a support ticket
  with Crazy Domains to complete DS record addition

## Evidence

Screenshots in `Evidence` folder: Cloudflare DNSSEC settings page,
Crazy Domains Name Servers/Administration tabs showing no DS
record option.
