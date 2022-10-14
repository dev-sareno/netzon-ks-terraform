# netzon-ks-terraform
Netzon knowledge sharing on Terraform and Cloud Infrastructure automation

## Requirements
1. Properly installed Terraform CLI *([installation guide](https://learn.hashicorp.com/tutorials/terraform/install-cli))*
1. IAM User with `AdministratorAccess` permission *(given permission is for demo purposes only, adjust accordingly)*
1. AWS CLI Access Keys
    ```shell
    $ export AWS_ACCESS_KEY_ID=**************
    $ export AWS_SECRET_ACCESS_KEY=**************
    $ export AWS_DEFAULT_REGION=us-east-1
    ```
    or run
    ```shell
    $ aws configure
    ```
1. AWS S3 bucket where Terraform state will be saved. To create, run
    ```shell
    $ aws s3api create-bucket --bucket netzon-ks-terraform
    ```

## Terraform

### Initialize
Run
```shell
$ terraform init
```

### Plan
Run
```shell
$ terraform plan
```

### Create Resources
Run
```shell
$ terraform apply --auto-approve
```

### Update/Fix config drifts
Run
```shell
$ terraform apply --auto-approve
```

### Destroy Resources
Run
```shell
$ terraform destroy --auto-approve
```
