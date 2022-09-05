# Deny Access to Unused regions

This Service Control Policy (SCP) restricts all access to unused regions, if one your AWS account gets compromised an attacker could spin up services on regions that you usually don't use, it could be hard to detect if someone is spinning up resources on another region, this SCP will lock any other region rather than your main one.

Some of the AWS services are exlcuded (global services): AWS IAM, AWS Organizations, AWS Route53, AWS Budgets, AWS WAF, AWS CloudFront, AWS Global Accelrator, AWS Snowball (Import/Export), AWS Support, AWS Health Dashboard, and Route53 Domain Registrations.

**Note:

Replace the line 51 with the name of your main region or add more if necessary.