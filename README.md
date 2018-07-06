# terraform-aws-cloudwatch-slack-integration

Manage AWS Cloudwatch to Slack notification integration

- Create lambda to communicate with Slack
  - Parse SNS Topic name to get Slack channel to send to

- Per service
  - Create SNS topic with Slack channel name in SNS topic name (Slack-<channel>)
  - Subscription: Lambda

- Outputs
  - SNS Topic: Name, ARN

  Alarms will use SNS topic to send to Slack

  AWS bas a basic blueprint to start lambda from
