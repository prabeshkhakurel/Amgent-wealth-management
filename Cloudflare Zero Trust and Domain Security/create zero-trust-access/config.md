# Cloudflare Zero Trust Access Policies

**Task:** Configure Cloudflare Zero Trust access policies
**Jira Task:** KAN-30
**Status:** Partially Done

## What was done

- Created a Gateway DNS policy to block malicious/unknown domains:
  - Traffic type: DNS
  - Condition: Security Categories in [malware, phishing, security
    risks / newly seen domains]
  - Action: Block
  - Policy status: Active

## Remaining

- Identity-based access policies requiring SSO integration with
  Microsoft Entra ID — pending confirmation of Entra ID/Conditional
  Access setup status (dependency on Prabesh's part of the project)
