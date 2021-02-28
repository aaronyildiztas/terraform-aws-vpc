# terraform-aws-vpc
terraform-aws-vpc

###  Requirements

#### Please user terraform 0.14.7 or above

### Please copy and paste the below code
```
module "vpc" {
  source = "aaronyildiztas/vpc/aws"
  region        = "us-east-1"
  cidr_block    = "10.0.0.0/16"
  public_cidr1  = "10.0.101.0/24"
  public_cidr2  = "10.0.102.0/24"
  public_cidr3  = "10.0.103.0/24"
  private_cidr1 = "10.0.1.0/24"
  private_cidr2 = "10.0.2.0/24"
  private_cidr3 = "10.0.3.0/24"
  tags = {
    Name    = "VPC"
    Team    = "DevOps"
    Billing = "CFO"
    Quarter = "3"
    AppName = "Wordpress"
  }
}

```
### Please run
```
terraform init
terraform apply
```
