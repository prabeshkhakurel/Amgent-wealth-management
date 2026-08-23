# SPF, DKIM, DMARC Configuration

**Task:** Set up SPF, DKIM, DMARC records
**Jira Task:** KAN-28
**Status:** In Progress

## Findings

- SPF record present and correctly configured for Microsoft 365:
  `v=spf1 include:spf.protection.outlook.com -all`
- DKIM records present for Mailchimp (dkim2.mcsv.net,
  dkim3.mcsv.net) and SMTP2GO (dkim.smtp2go.net) — no Microsoft
  365 DKIM selector record found yet, needs checking in the M365
  admin center
- DMARC record present but set to `p=none` — this means DMARC is
  currently monitor-only and not actively blocking spoofed email
- Recommend reviewing DMARC reports, then upgrading policy to
  `p=quarantine` or `p=reject` once confident legitimate mail
  won't be affected

## Evidence

Screenshot in `Evidence` folder: Cloudflare DNS records list
showing SPF, DKIM, and DMARC TXT records.
