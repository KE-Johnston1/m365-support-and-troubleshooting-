Identity and MFA Troubleshooting
Scenario
User lost access to Authenticator app

What the user reports
“I got a new phone and can’t sign in anywhere.”

Steps taken
Verify identity
Reset MFA in Azure AD
Guide user through re enrolment
User signs in successfully

Scenario
Account locked after repeated password attempts

What the user reports
“I keep getting locked out every morning.”

Steps taken
Unlock account in Azure AD
Check sign in logs
Identify repeated failures from an old device
Clear saved credentials
User signs in without issues

Scenario
User cannot complete MFA due to Conditional Access policy

What the user reports
“I get blocked every time I try to sign in.”

Steps taken
Check sign in logs
Identify Conditional Access policy blocking sign in
Add user to exclusion group temporarily
User signs in successfully
Review policy for long term fix

Scenario
User repeatedly locked out due to legacy authentication

What the user reports
“I keep getting locked out even after resetting my password.”

Steps taken
Check sign in logs
Identify repeated failures from an old device
Disable legacy authentication for the user
Clear saved credentials
User remains signed in without further lockouts

Scenario
User cannot access Microsoft 365 after licence change

What the user reports
“I was moved to a new licence and now nothing works.”

Steps taken
Check licence assignment
Force a re sync
Sign user out of all sessions
User signs in again
Apps load normally
