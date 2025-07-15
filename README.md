# AWS Account Creation Guide
##  Complete Step-by-Step Tutorial
### Phase 1: Account Setup
### (Creating your AWS root account)

## 1. Access AWS Console
Go to aws.amazon.com/console → Click "Create an AWS Account"
![](./img/1.%20AWS%20Console%20to%20create%20account.jpg/)

The AWS Management Console is your control panel for all cloud services.

## 2. Enter Account Details
Root Email: Use a dedicated email (e.g., admin@yourdomain.com)
Account Name: e.g., JV-IMPACTVR-INITIATIVE-LTD-GTE

Click "Verify Email Address"
![](./img/2.%20Sign%20Up.jpg)


Why?
The root account has full admin privileges - protect this email!

Phase 2: Verification
(Confirming your identity)

## 3. Email Verification
Check your email for OTP (e.g., 2556)

Enter code in AWS verification screen
![](./img/3.%20Choosing%20a%20free%20plan.jpg)

Why?
AWS uses OTP to prevent automated bot signups.

## 4. Set Root Password
Create a strong 12+ character password with:

Uppercase letters

Numbers

Special symbols (!@#$%)
Why?
This protects your root account from brute-force attacks.

Phase 3: Account Configuration
(Selecting your plan and payment)

## 5. Choose Account Plan
Select "Free (6 months)" to access:

$200 usage credits

750 EC2 hours/month

5GB S3 storage

15GB bandwidth
![](./img/3.%20Choosing%20a%20free%20plan.jpg)

Why?
Free tier lets you explore AWS without immediate costs.

## 6. Add Payment Method
Enter valid credit card:

AWS places $1 temporary hold (refunded in 3-5 days)

No charges unless you exceed free tier limits
Why?
Required for identity verification and potential usage beyond free tier.

Phase 4: Final Activation
(Completing your setup)

## 7. Phone Verification
Enter mobile number

Input SMS OTP code
Why?
Adds an extra layer of security through multi-factor verification.

## 8. Account Activation
Wait 1-3 minutes for confirmation:
![](./img/6.%20Congratulations.jpg)
Next Steps:

Check for "Welcome to AWS" email

Access console at https://console.aws.amazon.com

Phase 5: Post-Creation Security
(Protecting your account)

## 9. Enable MFA
Go to IAM → Users → Security Credentials

Assign virtual MFA device (Google Authenticator/Authy)

Diagram
Code

Why?
Prevents unauthorized access even if password is compromised.

## 10. Create IAM Admin User
Never use root for daily tasks!

IAM → Users → "Add User"

Name: Admin

Permissions: Attach AdministratorAccess policy
Why?
Limits exposure of root account credentials.

## 11. Set Billing Alerts
Billing Dashboard → Preferences

Enable "Receive Billing Alerts"

Create CloudWatch alarm at 80% of free tier limit

Why?

Avoids unexpected charges by notifying you before exceeding limits.

Free Tier Services
Service	Free Limit	Use Case
EC2	750 hrs/month	Virtual servers
S3	5GB storage	File storage
Lambda	1M requests	Serverless functions
RDS	750 hrs/month	Managed databases
CloudFront	50GB transfer	Content delivery
Troubleshooting Guide
Issue	Solution
OTP not received	Check spam folder; request new code after 10 mins
Payment declined	Use card supporting international transactions
"Pending Verification"	Contact AWS Support
Free tier not active	Confirm plan selection; wait 24 hours
