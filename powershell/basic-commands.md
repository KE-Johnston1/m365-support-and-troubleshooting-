Scenario
Check user licence details

Command
Get MgUserLicenseDetail -UserId user@domain.com
Why it’s useful
Quick way to confirm if missing features are caused by licence issues.

Scenario
List all devices registered to a user

Command
Get MgDevice -Filter "registeredOwners/any(x:x/id eq 'USER-ID')"
Why it’s useful
Helps identify stale or duplicate devices causing sign in problems.

Scenario
Reset MFA methods

Command
Reset MgUserAuthenticationMethod -UserId user@domain.com
Why it’s useful
Used when a user loses their phone or cannot complete MFA.

Scenario
Find all users without MFA enabled

Command
Get MgUserAuthenticationMethod -UserId user@domain.com
Why it matters
Helps identify accounts at risk and supports MFA rollout.

Scenario
Check sign in logs for a specific user

Command
Get MgAuditLogSignIn -Filter "userPrincipalName eq 'user@domain.com'"
Why it matters
Useful for diagnosing lockouts, MFA failures, and suspicious activity.

Scenario
List all devices that have not synced in 30 days

Command
Get MgDevice | Where-Object {$_.approximateLastSignInDateTime -lt (Get-Date).AddDays(-30)}
Why it matters
Helps identify stale devices that may cause authentication issues.
