# Deploy AWS Lambda to VPC with Terraform

Usage:

```bash
docker run --rm -it -v $(pwd):/var/app -w /var/app --entrypoint bash amazon/aws-cli
```

```bash
aws configure
```

```bash
yum install -y yum-utils
```

```bash
yum-config-manager --add-repo https://rpm.releases.hashicorp.com/AmazonLinux/hashicorp.repo
yum -y install terraform
```

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
