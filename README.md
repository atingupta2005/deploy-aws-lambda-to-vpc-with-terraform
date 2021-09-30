# Deploy AWS Lambda to VPC with Terraform

Usage:

```bash
cd terraform

terraform init
```

```bash
terraform apply
```

Invoke Lambda:

```bash
aws lambda invoke --function-name lambda-vpc-tf-lambda-function out.txt
{
    "StatusCode": 200,
    "ExecutedVersion": "$LATEST"
}
```

```bash
cat out.txt
"If you spell Chuck Norris in Scrabble, you win. Forever."
```
