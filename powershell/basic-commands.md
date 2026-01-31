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
