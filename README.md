A simple terrform script for provisioning ec2 instance on AWS and creating a CICD pipeline for the same.

Reference: https://www.youtube.com/watch?v=7xngnjfIlK4&t=1327s

## Install Terraform

Official installation instructions from HashiCorp: https://learn.hashicorp.com/tutorials/terraform/install-cli

## AWS Account Setup

AWS Terraform provider documentation: https://registry.terraform.io/providers/hashicorp/aws/latest/docs#authentication

1) create non-root AWS user
2) Add the necessary IAM roles (e.g. AmazonEC2FullAccess)
3) Save Access key + secret key (or use AWS CLI `aws configure` -- https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html)

## Hello World

`./main.tf` contains minimal configuration to provision an EC2 instance.

1) `aws configure`
2) `terraform init`
3) `terraform plan`
4) `terraform apply`