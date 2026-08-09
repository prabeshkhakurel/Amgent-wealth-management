# Microsoft Defender Testing

## Objective

Verify that all Microsoft Defender security controls are functioning correctly.

## Test Cases

| Test ID | Security Control | Test Procedure | Expected Result | Status |
|---|---|---|---|---|
| T01 | Microsoft Defender | Verify Defender is enabled and accessible | Defender security services are available | Pending |
| T02 | Safe Links | Verify Safe Links policy and test approved URL protection method | URLs are checked according to configured policy | Pending |
| T03 | Safe Attachments | Verify Safe Attachments policy using an approved test method | Suspicious attachments are detected or quarantined according to policy | Pending |
| T04 | Anti-Phishing | Verify anti-phishing policy and use an approved simulation/test method | Simulated phishing activity is detected according to policy | Pending |
| T05 | Anti-Spam | Review inbound spam protection | Spam messages are filtered according to policy | Pending |
| T06 | Security Alerts | Review Defender alerts after approved testing | Relevant security events are recorded where applicable | Pending |

## Current Testing Status

Testing has not yet been performed because access to the client's Microsoft 365 environment is pending.

The test cases have been prepared in advance so that security controls can be validated once the required administrative access is available.

## Evidence Required

- Screenshots of configured security policies
- Screenshots/results from approved security tests
- Defender alerts or reports generated during testing
- Final test results
- Jira updates documenting completed testing

## Safety Note

Testing will only be conducted using approved Microsoft testing or simulation methods. No real malware or malicious phishing content will be used.

## Overall Status

**Pending Client Access**
