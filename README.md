# CloudFormation-AWS
This repo contains templates used to create VPCs, Security Groups and EC2 instances on AWS

![image](https://user-images.githubusercontent.com/52250306/162491050-60b0e757-fe8d-413d-b123-124ff7993b70.png)

  This template document called create-vpc.yml will create a VPC as shown in the diagram, the VPC will contain different CIDR blocks. 

  Another template document called create-sg.yml will make a security group with two rules: allow SSH from a public space and allow HTTP from a public space.

  Finally the last template document called create-ec2.yml will create one EC2 instance with the ability of being located in any subnet in the new VPC and use the security groups created by the stack create-sg.yml 
