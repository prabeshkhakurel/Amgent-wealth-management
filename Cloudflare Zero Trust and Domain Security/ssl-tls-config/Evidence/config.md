# SSL/TLS Configuration

**Task:** Configure SSL/TLS mode (Full Strict)
**Jira Task:** KAN-27
**Status:** In Progress

## Findings

- Current Cloudflare SSL/TLS encryption mode: Full
- Scope of work requires Full (Strict), not just Full
- Full Strict validates that the origin server has a trusted SSL
  certificate, closing a gap where traffic between Cloudflare and
  the origin server could otherwise be intercepted
- Not yet changed — upgrading to Full Strict on a live client
  domain risks breaking the site if the origin server's
  certificate isn't valid, so this is pending team/supervisor
  sign-off before changing
- No live traffic recorded in the last 24 hours at time of review,
  which lowers (but does not eliminate) the risk of testing this

## Evidence

Screenshot in `Evidence` folder: Cloudflare SSL/TLS Overview page
showing current mode set to Full.
