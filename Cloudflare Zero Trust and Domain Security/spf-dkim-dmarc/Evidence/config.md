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

  ## Update (today's session)

- Attempted to verify Microsoft 365 DKIM selector configuration
  via admin.microsoft.com — do not currently have working admin
  access. Need credentials from team/Ben to proceed.

## Evidence

Screenshot in `Evidence` folder: Cloudflare DNS records list
showing SPF, DKIM, and DMARC TXT records.

## Update — DKIM enabled

- Confirmed Microsoft 365 DKIM was disabled (NoDKIMKeys status)
  for amgentwealth.com.au
- Added required CNAME records to Cloudflare:
  - selector1._domainkey → selector1-amgentwealth-com-au._domainkey.amgentwealth.w-v1.dkim.mail.microsoft
  - selector2._domainkey → selector2-amgentwealth-com-au._domainkey.amgentwealth.w-v1.dkim.mail.microsoft
- Successfully enabled DKIM signing in Microsoft Defender
- Status: DKIM now Enabled for Microsoft 365 mail
- Remaining: review DMARC policy (currently p=none)

- ## Update — DMARC review

- Reviewed DMARC reports via Cloudflare Email > DMARC Management
- Last 7 days: 78 emails passed DMARC, 16 failed
- Microsoft Corporation (legitimate M365 mail): 97.4% pass rate
- Google LLC: 0% pass (11 emails) — source unconfirmed
- Amazon.com, Inc.: 0% pass (2 emails) — source unconfirmed
- Servers Australia Pty Ltd: 75% pass (4 emails)
- Decision: holding off on tightening DMARC policy (p=none →
  p=quarantine) until confirming with Ben whether Google/Amazon
  services are legitimately used to send mail on his behalf

  ## Update — DMARC moved to enforcement

- Changed DMARC policy from p=none to p=quarantine
- Reasoning: legitimate Microsoft 365 mail passes at 97.4%,
  unverified failing senders (Google LLC, Amazon.com Inc) could
  not be confirmed as legitimate by Ben/team — treated as
  potential spoofing risk per DMARC best practice
- New record: v=DMARC1; p=quarantine; rua=mailto:...; pct=100;
- Next: monitor reports, consider p=reject after a stable period
- Status: Done

