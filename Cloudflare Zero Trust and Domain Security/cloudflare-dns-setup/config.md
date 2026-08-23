# Cloudflare Account Setup & DNS Migration

**Task:** Add domain to Cloudflare and update nameservers
**Jira Task:** KAN-25
**Status:** Done

## Findings

- Nameservers already pointed to Cloudflare
  (mario.ns.cloudflare.com / monika.ns.cloudflare.com) — migration
  was already completed prior to this review
- DNS Setup mode: Full (13 of 200 DNS records in use)
- Records reviewed: A record, MX (Microsoft 365), autodiscover
  CNAME, DKIM records (Mailchimp, SMTP2GO), SPF, DMARC, www CNAME
- SPF record present and correctly configured for Microsoft 365
- DMARC record present but set to p=none (monitor-only, not
  enforcing) — flagged for review

## Evidence

Screenshots in `Evidence` folder: Cloudflare DNS records list,
Name Servers tab in Crazy Domains confirming Cloudflare NS.
