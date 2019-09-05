# Terraform AWS Common IAM Policies
[![Terraform Version](https://img.shields.io/badge/Terraform%20Version->=0.11.14,_<0.12.0-blue.svg)](https://releases.hashicorp.com/terraform/)
[![Release](https://img.shields.io/github/release/traveloka/terraform-aws-common-iam-policies.svg)](https://github.com/traveloka/terraform-aws-common-iam-policies/releases)
[![Last Commit](https://img.shields.io/github/last-commit/traveloka/terraform-aws-common-iam-policies.svg)](https://github.com/traveloka/terraform-aws-common-iam-policies/commits/master)
[![Issues](https://img.shields.io/github/issues/traveloka/terraform-aws-common-iam-policies.svg)](https://github.com/traveloka/terraform-aws-common-iam-policies/issues)
[![Pull Requests](https://img.shields.io/github/issues-pr/traveloka/terraform-aws-common-iam-policies.svg)](https://github.com/traveloka/terraform-aws-common-iam-policies/pulls)
[![License](https://img.shields.io/github/license/traveloka/terraform-aws-common-iam-policies.svg)](https://github.com/traveloka/terraform-aws-common-iam-policies/blob/master/LICENSE)

This repository is a collection of IAM Policies that are commonly used in Traveloka. The resource created by each module inside [modules](https://github.com/traveloka/terraform-aws-common-iam-policies/tree/master/modules) directory is only IAM Policy. You need to provision IAM Role separately, and then attach the policy to the role.

## Table of Content

- [Dependencies](#Dependencies)
- [Quick Start](#Quick-Start)
- [Versioning](#Versioning)
- [Contributing](#Contributing)
- [Authors](#Authors)
- [License](#License)

## Dependencies

This module has no dependency. But to make it works, you may need an [IAM Role module](https://registry.terraform.io/modules/traveloka/iam-role)

## Quick Start

Open [examples](https://github.com/traveloka/terraform-aws-common-iam-policies/tree/master/examples) directory and choose one. See the README file for the example and follow the `usage` information.

## Versioning

Please also see our [CHANGELOG.md](./CHANGELOG.md) for full details.

## Contributing

Contributions are welcomed! See [CONTRIBUTING.md](./CONTRIBUTING.md) for full details.

## Authors
- [S. Shvetsov](https://github.com/sshvetsov)
- [Ronny Kaluge](https://github.com/ronny-kaluge)
- [Rafi Kurnia Putra](https://github.com/rafikurnia)

## License

Apache 2 Licensed. See [LICENSE](./LICENSE) for full details.
