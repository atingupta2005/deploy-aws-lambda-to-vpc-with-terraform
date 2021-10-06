# Deploy AWS Lambda to VPC with Terraform

Usage:

```bash
git clone https://github.com/atingupta2005/deploy-aws-lambda-to-vpc-with-terraform.git
cd terraform
```

```
terraform init
```

```
terraform apply -auto-approve
```

Invoke Lambda:

```
aws lambda invoke --function-name lambda-vpc-tf-lambda-function out.txt
```

```bash
cat out.txt
```
