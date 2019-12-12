
# Cloud Foundation Toolkit Lab - Getting Started

## **Prerequisite**

Complete **Setup** Labs

You should have [Google Cloud SDK](https://cloud.google.com/sdk/docs/downloads-interactive) installed and configured before continuing, otherwise refer to [00-Setup/README.md](../../00-Setup/README.md)

## Identity and Access Management

This lab helps you create IAM role bindings using Cloud Foundation Toolkit.

At the end of the exercise, you will users in your projects that have been granted access to resources within GCP.

**Note**: You can have input variables as

* **default** in `variables.tf`
* using [terraform.tfvars](https://www.terraform.io/docs/configuration/variables.html#variable-definitions-tfvars-files)
* command line argument `-var='key=value'`

### What You’ll Learn

* [IAM](https://cloud.google.com/iam/docs/overview)
* [Cloud Foundation Toolkit](https://cloud.google.com/foundation-toolkit/)
* [terraform-google-iam](https://github.com/terraform-google-modules/terraform-google-iam)


## Task 1. Create IAM Role Bindings

Use the Cloud Foundation Toolkit [IAM module](https://github.com/terraform-google-modules/terraform-google-iam) in `main.tf` to setup role bindings for a *user* and a *group*.


## Task 2. Terraform

### Terraform Init & Plan

Init and validate Terraform execution plan

```
terraform init
terraform plan -out=plan.out
```

### Terraform Apply

Execute previous generated execution plan

```
terraform apply plan.out
```

## Task 3. Verify
On Google Cloud Console, nagivate to **IAM & admin -> IAM**

Review the user permissions under **Members**
