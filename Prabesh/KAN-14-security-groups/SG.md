
Create a pilot security group in Microsoft Entra ID for security testing.
# KAN-14 – Security Pilot Group

## Objective
Create a dedicated Microsoft Entra security group for controlled testing of Microsoft 365 and Entra ID security policies before production deployment.

## Group Name
AMG-Security-Pilot

## Group Type
Security

## Membership Type
Assigned

## Work Completed
- Reviewed the existing Microsoft Entra groups.
- Created the AMG-Security-Pilot security group.
- Configured the group as a Security group with Assigned membership.
- Added the AMGENT Security Test account as a member.
- Verified that the test account was successfully added as a direct member.

## Purpose
The AMG-Security-Pilot group was created to provide a controlled testing environment.

Security policies such as Microsoft Authenticator and Conditional Access can be assigned to this group first instead of applying them directly to the production user.


## Testing and Verification
The AMG-Security-Pilot group was visible in Microsoft Entra after creation.

The group membership was reviewed and the AMGENT Security Test account was confirmed as a direct member.

## Result
The pilot security group was successfully created and prepared for security-policy testing.

## Status
Completed
