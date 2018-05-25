# RMISC-AWS-Security-Best-Practices-2018-05-10
AWS Security Best Practices presentation given at the Rocky Mountain Information Security Conference on 5/10/18

Here is the presentation that I gave at this conference.
The other part of this presentation was a live demonstration running in AWS with many of the security features enabled.

The AWS environment was based on the NIST QuickStart Templates.
https://aws.amazon.com/quickstart/architecture/accelerator-nist/

Picture of the AWS Sandbox Account.

![alt tag](https://github.com/ScottHogg/RMISC-AWS-Security-Best-Practices-2018-05-10/raw/master/Testbed%20AWS%20Account.jpg)

The AWS WAF was configured with the rules that came from the AWS WAF Security Automations:
https://aws.amazon.com/answers/security/aws-waf-security-automations/
Here are some URLs that you can use to test your WAF.
https://www.hoggcloud.com/foo?username=1' or '1' = '
https://www.hoggcloud.com/foo?username=1%27%20or%20%271%27%20=%20%27
https://www.hoggcloud.com/(\.|(%|%25)2E)(\.|(%|%25)2E)(\/|(%|%25)2F|\\|(%|%25)5C)/i

Simply follow these instructions and deploy the CFT into your account, in the region with your ALB.
https://docs.aws.amazon.com/solutions/latest/aws-waf-security-automations/deployment.html

Kali Linux can be downloaded and installed into your account from the AWS Marketplace.
https://aws.amazon.com/marketplace/pp/B01M26MMTT/

Some of the AWS event-driven security examples I showed came from this tutorial and this example.

Tutorial: Log Amazon S3 Object-Level Operations Using CloudWatch Events
http://docs.aws.amazon.com/AmazonCloudWatch/latest/events/log-s3-data-events.html

Event-Driven AWS Security: A Practical Example
https://securosis.com/blog/event-driven-security-on-aws-a-practical-example

I also showed how Duo CloudMapper can help diagram out your AWS environment.
https://duo.com/blog/introducing-cloudmapper-an-aws-visualization-tool
https://github.com/duo-labs/cloudmapper

Prowler is also a great way to check compliance of your AWS account.
https://github.com/Alfresco/prowler
