# Terraform_aws-resources

You can use it for :

# 1. Create VPC
# 2. Create Internet Gateway
# 3.Create a Custom Route Table
# 4. Create a Subnet
# 5. Associate subnet with route Table.
# 6. Create a security group to allow port 22,80,443
# 7. Create a network interface with an ip in the subnet that was created in step 4
# 8. Assign an elastic IP to the network interface created in step 7
# 9. Create ubuntu Server and install/enable apache2

*Note: You have to enter your access_key & secret_key for aunthentication*

# Commands you have to use to run this file

1. terraform init - It’s the first command you need to execute. Unless  terraform plan , apply  , destroy   and import  will not work. The command terraform init   will install :

Terraform modules
Eventually a backend
Provider(s) plugins

2. terraform plan -It’s an important feature of Terraform that allows a user to see which actions Terraform will perform prior to making any changes, increasing confidence that a change will have the desired effect once applied.

When you execute terraform plan, Terraform will scan all *.tf files in your directory and create the plan.

3. terraform apply -ince Terraform v0.11+, in an interactive mode (non CI/CD/autonomous pipeline), you can just execute terraform apply command which will print out which actions TF will perform.

By generating the plan and applying it in the same command, Terraform can guarantee that the execution plan won’t change, without needing to write it to disk. This reduces the risk of potentially-sensitive data being left behind, or accidentally checked into version control.
