<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Build a Virtual Private Cloud

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-networks-vpc)

**Author:** saqibh49@gmail.com  
**Email:** saqibh49@gmail.com

---

## Build a Virtual Private Cloud (VPC)

![Image](http://learn.nextwork.org/grateful_white_lucky_bat/uploads/aws-networks-vpc_2facf927)

---

## Introducing Today's Project!

In this project, I will demonstrate how to create a VPC (Virtual Private Cloud), set up Subnets and create an internet gateway. I'm doing this project to learn more about the capabilities of AWS and get a better understanding of some of the things I can do with AWS.

### What is Amazon VPC?

Amazon VPC is a space separate from the general internet that allows for data to stored in a private place while still being able to connect to internet connected items also in the VPC 

In today's project, I used Amazon VPC to create a VPC, then a subnet, and finally an internet gateway.

### Personal reflection

This project took me about 2-3 hours

One thing I didn't expect in this project was to learn a bit about using the command line. It was a great time, and I'm hoping to get more comfortable with it in the future.

---

## Virtual Private Clouds (VPCs)

### What I did in this step

In this step, I will access the VPC console and create my first VPC.

### How VPCs work

VPCs are private spaces and essentially folders that organize the AWS cloud so all files aren't scattered throughout the cloud and always public

### Why there is a default VPC in AWS accounts

There was already a default VPC in my account ever since my AWS account was created. This is because AWS automatically loads default VPCs in every account so users get started with tools like EC2 right away

![Image](http://learn.nextwork.org/grateful_white_lucky_bat/uploads/aws-networks-vpc_2facf927)

### Defining IPv4 CIDR blocks

To set up my VPC, I had to define an IPv4 CIDR block, which is a way to assign IP adresses to my VPC. By assigning IP addresses, I'm telling AWS what range of addresses are considered within my VPC. 

---

## Subnets

### What I did in this step

In this step, I will set up subnets within my VPC because this helps organize it into different spaces which can help with organization and structure.

### Creating and configuring subnets

Subnets are like neighborhoods in the city that is my VPC. There are already subnets existing in my account, one for every Availability Zone in my region.

### Public vs private subnets

The difference between public and private subnets are public subnets can be accessed from the internet, whereas private subnets stay in the backend, not able to be accessed through the internet. For a subnet to be considered public, it has to be connected to an internet gateway.

![Image](http://learn.nextwork.org/grateful_white_lucky_bat/uploads/aws-networks-vpc_157c4219)

### Auto-assigning public IPv4 addresses

Once I created my subnet, I enabled the option to Auto-Assign Public IPv4 Addresses. This setting makes sure that anytime an EC2 instance gets built within my subnet, it automatically gets a public IP so that I don't have to manage that separately for each instance.

---

## Internet gateways

### What I did in this step

In this step, I will create an internet gateway because that is how my VPC can connect with the rest of the internet.

### Setting up internet gateways

Internet gateways are how VPCs connect with the rest of the internet.

Attaching an internet gateway to a VPC means the contents of my VPC can access the internet and users on the internet can view the contents of my VPC. If I missed this step my VPC and all it's contents would only be accessible internally.

![Image](http://learn.nextwork.org/grateful_white_lucky_bat/uploads/aws-networks-vpc_4ae90410)

---

## Using the AWS CLI

### What I'm doing in this extension

In this project extension, I will use AWS Cloudshell and AWS CLI to do the same task of creating a VPC, a ssubnet and an internet gateway because it may be a faster way of doing the same job

### Exploring CloudShell and CLI

### Debugging my setup

To set up a VPC or a subnet, you can use the aws ec2 create-vpc or aws ec2 create-subnet command. Make sure to avoid errors by including a valid --cidr-block that fits within the VPC range and meets AWS minimum size requirements.

![Image](http://learn.nextwork.org/grateful_white_lucky_bat/uploads/aws-networks-vpc_9b2465411)

### Comparing CloudShell vs AWS Console

Compared to using the AWS Console, an advantage of using commands is that it gives you a lot more control over what you're doing. advantage of using the Console is it's a lot faster than using the AWS interface. Overall, I preferred using the interface but I think as I get used to the command line, I'll end up preferring that more. 

---

---
