

# KAN-13 – Conditional Access

## Objective
Configure and test a Conditional Access MFA policy using the pilot environment before production enforcement.

## Policy Name
CA-PILOT-Require-MFA

## Pilot Group
AMG-Security-Pilot

## Target Resources
All resources

## Grant Control
Require multifactor authentication

## Location
Any location

## Policy State
Report-only

## Work Completed
- Created the CA-PILOT-Require-MFA Conditional Access policy.
- Assigned the AMG-Security-Pilot group.
- Configured all resources as the target.
- Configured multifactor authentication as the access requirement.
- Kept the policy in Report-only mode for safe pilot testing.
- Tested sign-in using the AMGENT Security Test account.
- Reviewed Microsoft Entra sign-in logs.
- Reviewed the Conditional Access Report-only result.

## Testing Result
The AMGENT Security Test account generated successful sign-in events.

The CA-PILOT-Require-MFA policy was evaluated in Report-only mode and showed that user action would be required if the policy were enforced.

## Security Consideration
Report-only mode was used to reduce the risk of locking out the production user during testing.

Microsoft Entra also displayed a warning that Security Defaults must be disabled before Conditional Access can be enforced. No production enforcement was performed at this stage.

## Current Status
Pilot Conditional Access testing completed.

Production enforcement remains pending.

## Remaining Work
- Create and test the compliant-device Conditional Access policy.
- Complete final pilot validation.
- Register MFA on Ben's own phone.
- Prepare controlled production rollout.
