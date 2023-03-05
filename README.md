<div align="center">
#create gif and update this
<img src="https://raw.githubusercontent.com/turnertime42/terraform-localstack-awscostestimator/main/main.tf" width="100%"/>


</div>




## Introduction

This was an initial go at creating this so there is much to be desired. It basically helps people looking to get a cost estimate of what their IAAS/SAAS/PAAS would be on AWS via mocked resources in localstack sans networking costs(egress, etc)

For future I'd like to integrate terraform graph as well to give a logical diagram along with a few other open source tools(checkov, terratest, terragrunt, etc)

You can add new resources as you see fit for your specific use case and probably split out/refactor them for a better layout. For a quick and dirty AWS billing estimate though this will get you on your way.




## Requirements and Dependencies

- Install Docker Desktop. See [Docker Desktop Website](https://www.docker.com/products/docker-desktop/) for full documentation and useful links.
- Install localstack docker extension. See [LocalStack extension Website](https://github.com/localstack/localstack-docker-extension)  for full documentation and useful links.
- I use [VScode](hhttps://code.visualstudio.com/download) for my personal code editor since it has tons of extensions but you're free to use whatever.
- Install terraform cli. See [terraform docs](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli) for instructions.
- Install [awscli](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html) to interact with mocked aws services.
- Start Docker Desktop and launch the latest localstack docker instance via the extension.

## Other Useful Links

- [LocalStack AWSCLI](https://docs.localstack.cloud/user-guide/integrations/aws-cli/)

## Features

- Emulated AWS Infrastructure
- Billing estimate of mocked AWS infrastructure
- Horrible initial code

[See all features →](https://youtu.be/dQw4w9WgXcQ)

## Example Commands

Clone Repo:

```bash
git clone {repo_name}
```

Initialize terraform:

```bash
terraform init
```

Create the plan:

```bash
terraform plan -out=tfplan
```

Apply the plan to get cost estimate of infrastructure:

```bash
terraform apply
```

Share the cost results!


[See more examples →](https://www.youtube.com/watch?v=K8pdB8X7kIks)
