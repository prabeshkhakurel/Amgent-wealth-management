
# KAN-10 – Document Microsoft 365 Users and Administrators

## Project

Amgent Wealth Management Security Upgrade

## Task

KAN-10 – Document Microsoft 365 Users and Administrators

## Objective

The objective of this task was to review and document the current Microsoft 365 user accounts and administrator roles before making security changes.

## Current Users

The Microsoft 365 Admin Center was reviewed.

Two active user accounts were identified:

| User | Account | Licence |
|------|---------|---------|
| Admin | admin@amgentwealth.com.au | Unlicensed |
| Ben Waite | ben@amgentwealth.com.au | Microsoft 365 Business Standard (no Teams), Microsoft Teams Essentials and Microsoft Power Automate Free |

## Administrator Roles

The administrator roles of the existing accounts were reviewed.

### Admin Account

The Admin account currently has the **Global Administrator** role.

### Ben Waite

Ben Waite currently has **Admin Center access** and the
**Global Administrator** role.


## Changes Made

No user accounts, licences or administrator roles were changed during
this task.



## Result

The current Microsoft 365 users and administrator roles were
successfully reviewed and documented.


## AFTER ACCESS

# KAN-10 – User and Administrative Access Review

## Objective
Review Microsoft 365 user accounts and administrative privileges before implementing security controls.

## Work Completed
- Reviewed the existing Microsoft 365 user accounts.
- Identified the production user and the AMGENT Security Test account.
- Reviewed administrative access for the pilot test account.
- Confirmed that the AMGENT Security Test account has no administrator access.
- Reviewed the production administrator account.
- Maintained the pilot account as a standard user for security testing.

## Security Principle
The AMGENT Security Test account was not given unnecessary administrative privileges.

Keeping the pilot account as a standard user supports the principle of least privilege and reduces the risk associated with excessive administrative access.

## Findings
- AMGENT Security Test: Standard user with no administrator access.
- Production administrator account: Administrative access reviewed.
- Pilot security testing was performed without granting unnecessary administrator privileges to the test account.

## Result
Microsoft 365 user accounts and administrative privileges were successfully reviewed.

The pilot account was confirmed to have no administrator access and was suitable for controlled security-policy testing.

## Status
Completed


