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

  ## Update (today's session)

- Cloudflare DNSSEC enabled; DS record generated:
  - Key Tag: 2371
  - Algorithm: 13
  - Digest Type: 2 (SHA256)
  - Digest: 9E3F93606339D48400B01A115BA23DA2B3D2D8BD4A94C71DC067A6DE8CB34B4
- Submitted these values to Crazy Domains support via live chat
- Automated support bot confirmed DS records require manual
  registrar-level publication but could not complete the action
- Next step: escalate to a human Crazy Domains support agent

## Evidence

Screenshots in `Evidence` folder: Cloudflare DNSSEC settings page,
Crazy Domains Name Servers/Administration tabs showing no DS
record option.
