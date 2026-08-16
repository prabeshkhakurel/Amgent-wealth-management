# Microsoft Defender and Email Security – Testing

**Team Member:** Kiran Pariyar  
**Project:** Amgent Wealth Cybersecurity Upgrade  
**Area:** Microsoft Defender and Email Security  

## Purpose

The purpose of this testing is to verify that Microsoft Defender and email security controls are correctly configured and working as expected after implementation.

## Planned Security Tests

| Test ID | Security Control | Test Method | Expected Result | Status |
|---|---|---|---|---|
| T01 | Microsoft Defender | Review Defender security status and active policies | Defender services and required protection are enabled | Planned |
| T02 | Safe Links | Send/test an email containing a safe test URL and verify Safe Links processing | URL protection policy is applied correctly | Planned |
| T03 | Safe Attachments | Perform an approved test using a safe test attachment | Attachment is scanned according to the configured policy | Planned |
| T04 | Anti-Phishing | Review and test the configured anti-phishing policy | Suspicious/phishing messages are detected or handled according to policy | Planned |
| T05 | Anti-Spam | Review inbound anti-spam policy and perform an approved test | Spam messages are handled according to the configured policy | Planned |
| T06 | Anti-Malware | Review malware protection policy and perform an approved Microsoft-supported test | Malicious test content is blocked or quarantined | Planned |
| T07 | Quarantine | Review quarantined messages after security testing | Detected threats appear in quarantine with the appropriate action | Planned |

## Evidence Required

Evidence will be collected during implementation and testing, including:

- Screenshots of Microsoft Defender configuration
- Safe Links policy screenshots
- Safe Attachments policy screenshots
- Anti-Phishing policy screenshots
- Anti-Spam and Anti-Malware configuration
- Test results
- Quarantine evidence where applicable

## Week 4 Status

Client administrative access has been received.

The Microsoft Defender and email security implementation has started. Baseline security settings will be reviewed and documented before configuration changes are made.

**Overall Testing Status:** Planned / Not Yet Completed

## Next Steps

1. Review the existing Microsoft Defender configuration.
2. Capture baseline screenshots.
3. Configure the required security policies.
4. Perform controlled security tests.
5. Record actual results in this document.
6. Add screenshots and other evidence.
7. Update each test status to Pass, Fail, or Requires Review.
