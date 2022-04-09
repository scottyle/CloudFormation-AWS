# CloudFormation Operation 

The fundamental building block of CloudFormation is the **stack**. A stack is the executed definition of a template, the stack builds the infrastructure using a template. Once the stack is deleted, all resources are deleted as well. 

A template is a declaration of AWS resources that make up a **stack**

# CloudFormation Stack Creation

Stack is the way CloudFormation uses to organize the resource instantiation. Refer to the image below to where the stack will be uploaded. For this repo we will be creating the template in yaml format using a text editor. 

![image](https://user-images.githubusercontent.com/52250306/162585477-fdc30c6c-4640-4cf6-b7f3-4038fab5a9a7.png)

# CloudFormation Lab 

![image](https://user-images.githubusercontent.com/52250306/162491050-60b0e757-fe8d-413d-b123-124ff7993b70.png)

  This repo contains templates used to create VPCs, Security Groups and EC2 instances on AWS

  This template document will be called create-vpc.yml will create a VPC as shown in the diagram, the VPC will contain different CIDR blocks one private and one public. The create-vpc will output the VPC-ID, Private and Public Subnet ID which the other stacks will reference. 

  Another template document called create-sg.yml will make a security group with two rules: allow SSH from a public space and allow HTTP from a public space. This template will reference the create-vpc stack. 

  Finally the last template document called create-ec2.yml will create 2 EC2 instances with the ability of being located in any subnet in the new VPC and use the security groups created by the stack create-sg.yml 
  
  
  
  
