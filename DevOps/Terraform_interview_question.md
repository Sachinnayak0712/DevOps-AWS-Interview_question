![featured](https://github.com/Sachinnayak0712/DevOps-AWS-Interview_question/assets/66566069/6e01f533-b609-4911-9466-2664d9cd6373)

# TERRAFORM INTERVIEW QUESTIONS

# Beginner
## what is terraform
Terraform, an open source “Infrastructure as Code” tool created by HashiCorp, allows programmers to build, change and version infrastructure safely and efficiently.
## Why Terraform is used for Devops
Terraform is an infrastructure as code (IaC) software tool that allows DevOps teams to automate infrastructure provisioning using reusable, shareable, human-readable configuration files. The tool can automate infrastructure provisioning in both on-premises and cloud environments.
## What is Terraform Init
Terraform initializes the code using the command terrafom init. this command  is used to initialize the working directory containing Terraform configuration file.\
Plugin Installation, Child Module Installation, Back-end Initialization
## How does Terraform works
![maxresdefault](https://github.com/Sachinnayak0712/DevOps-AWS-Interview_question/assets/66566069/45f093de-d301-4ae5-bdaf-fad1cdbcdd42)


There a 4 stages\
Terraform init - used to create a operational directory.\
Terraform plan - implements an execution strategy. \
Terraform apply - Ensures that the plan is set in motion in the timeframe. \
Terraform destroy - used to eliminate all the applied resources.
## Define null resources in Terraform
null resources implements standard resources library, but no further action is taken. The trigge t argument allows an orbitory set of valued the will cause the replacement of resources when changed.
## How does terraform work
## how to check the installed version Terraform
Launch powershell and enter terraform --version
## what is a provider in Terrafom? Enlist some Terraform Providers
Terraform provider is responsible for understanding API interactions and exposing resources
## Describe a few Terraform CLI commands and their functions
Terraform init, get, Graph, Validate, FMT
## What does HCL stands for
In Terraform HCL stands dor Hashicrop configureation Language. It is a configuration languages built by Hashicrop that is used to build a structured configuration languafe that is both human and machine- friendly for used with command-line tools but specifically targeted forword Devops tools
## what are modules in Terraform
A module in Terrafom is a container for several resources that are used together. The root modules is compulsory for every Terraformthat inclueds resources menstioned in the .tf files 
## What is Remote Backend in terraform
it is an extension that is used to state the status of terraform and also run the operations of terraform cloud. it has several commands to carry out all the the operations of terraform 
## Define IAC
Infrastucture As Code.\
A scheme whereby developers can run and provision the computer data centers mechanically instedof getting into a physical process.
## Resources Graph in Terraform
vistual representation of the resources andit helps create and modify the independent resources simuntaneously


## what is the use of FMT command in Terraform
It is used to rewrite Terraform configuratiion files to a canonical format and style. it allplies a subset of terraform language style conventions along with other minor adjustment for readability
## what are the ways to lock terraform module versions
## what does the following list of commands do.
Terraform -version - check the installed version of terraform.\
Terrafom destroys - to distroy the managed infrastructure of terraform.\
Terrafom fmt - it is used to rewrite configuration files in a canonical styles and format.\
Terraform provides - it gives information of provides working in the current configuration.

## what is terraform configuration for creating a single EC2 instance in AWS
provides "aws" {\
region = "ap-south-1" 
}\
resource "aws_instance"\
"enample" {\
ami = "ami-e4rd4t55"\
instance_type = "t2.micro"\
tags{\
Name="Terraform-Example"\
}\
}


## How would you recover form a failed apply in terraform
u can put ur config in version control and commit before each changes. than u can use ur version control system's features to revert to an older configuration is needed
## Terragrunt
Terragrunt is a covering layer that is used to cover terraform and is thin in nature. this layer helps to implement the practices that are advanced and vetted under terraform
## State File Locking
It is mechanism in Terraform where operation on specific state file is blocked to avoid conflicts between multiple users performing the same operation. 
