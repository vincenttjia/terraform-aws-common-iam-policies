# terraform-aws-common-iam-policies/datadog-integration
This module is meant to create an IAM Policy for AWS-Datadog integration.

## Usage

You can open this example:
- [Datadog Integration](https://github.com/traveloka/terraform-aws-common-iam-policies/tree/master/examples/datadog-integration)


## Important Notes

You need to:
1. go to https://app.datadoghq.com/account/settings#integrations/amazon_web_services and try to add an account, you will get an external ID (don't close the tab yet)
2. create an IAM Role using [traveloka/terraform-aws-iam-role](https://registry.terraform.io/modules/traveloka/iam-role/aws) module, and use this module to create the policy. Finally, attach the policy to the role using run this module using that external ID (Or you can open this [example](https://github.com/traveloka/terraform-aws-common-iam-policies/tree/master/examples/datadog-integration))
3. use your AWS Account ID and the generated AWS Role name to add an account at https://app.datadoghq.com/account/settings#integrations/amazon_web_services (at the same tab that give you the exernal ID)
4. fill the *"Per namespace"* section by clicking button *"Add an account specific namespace rule"* and choose which *"Service"* you **really need** to collect

Step (4) is very important, because we will update the *"Preferences for all accounts"* section **by 1 August 2019** to **not collect any AWS metrics**

Also important:
* fill the *"Optionally limit metrics collection"* section if not all instances in your AWS account need to get the metrics and EC2 tags streamed *from AWS*

  additional info: most (if not all) of necessary AWS EC2 metrics are already covered by Datadog agent

## Authors
- [Ronny Kaluge](https://github.com/ronny-kaluge)

## License
Apache 2 Licensed. See [../../LICENSE](../../LICENSE) for full details.
