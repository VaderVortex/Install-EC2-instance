# EX - 2:  Cloud Storage Creation (S3) And Launching an (EC2) Instance in AWS

## Aim:
Sign up for AWS. Visit AWS Console and create an account. Set up IAM roles and users with appropriate permissions. Navigate AWS Services. Log in to the AWS Management Console. Explore EC2, S3, IAM, RDS, VPC, and other key services. Understand AWS Free Tier Limits

## Algorithm:
Prepare Ubuntu Server (20.04/22.04)

Use a clean Ubuntu Linux environment (preferably a VM or EC2). Update & Install Dependencies

bash Copy Edit sudo apt update && sudo apt upgrade -y sudo apt install -y software-properties-common sudo add-apt-repository cloud-archive:wallaby -y sudo apt update Install OpenStack Services

bash Copy Edit sudo apt install -y openstack-client sudo apt install -y keystone glance nova-api nova-conductor nova-novncproxy nova-scheduler Configure Keystone (Identity Service)

Initialize Keystone, set up an admin user, and configure API endpoints. Install Glance (Image Service)

Enable support for OpenStack virtual machine images. Configure Nova (Compute Service)

Manage virtual instances inside OpenStack. Verify Installation

bash Copy Edit openstack --version openstack service list Launch OpenStack Dashboard

Access Horizon Dashboard using http:///dashboard. Log in with admin credentials.


## Procedure:
AWS offers a free tier with limited services. Ensure services used do not exceed free limits. Use AWS CLI

Install AWS CLI using pip install awscli or download from AWS. Configure AWS CLI using aws configure. Practice with AWS Documentation

![424431972-edae0a14-ef01-4e00-94ef-c51ed9033e5d](https://github.com/user-attachments/assets/0b9d1407-b9e3-492b-ab1b-92b66110304e)

Visit the AWS Documentation for hands-on learning. 2. Create & Manage Amazon EC2 Instances Algorithm:

Log in to AWS Console

Navigate to EC2 Dashboard. Launch an EC2 Instance

Click Launch Instance. Choose an Amazon Machine Image (AMI) (e.g., Ubuntu, Amazon Linux). Select an Instance Type (e.g., t2.micro for Free Tier). Configure Instance Details

Set up Networking (VPC, Subnet). Enable Auto-assign Public IP if needed. Add Storage

Set root volume size (e.g., 8GB default). Configure Security Group

Allow SSH (port 22), HTTP (port 80), or other required ports. Create & Download Key Pair

Select Create a new key pair and download .pem file. Launch the Instance

Click Launch and wait for initialization. Connect to the Instance

Open Terminal/Command Prompt.

![424432098-64db793c-7160-40b1-bd6f-2f8cd54487a8](https://github.com/user-attachments/assets/8563d788-f203-4dd6-a537-a67015537696)

Run ssh -i your-key.pem ec2-user@your-instance-ip. Result:

Successfully launched and connected to an EC2 instance. 3. Install OpenStack (OpenStack is an open-source cloud platform for managing virtualized resources.)



## Output:

![424432268-c74b31e6-e344-402b-90b0-c3861f48ad0c](https://github.com/user-attachments/assets/32654bfd-d732-4799-a28b-ccfb8b602a08)

![424432340-c26a835a-8110-43a2-af78-e7843306a23f](https://github.com/user-attachments/assets/ddc39873-604b-4afd-9211-65a73794045c)

## Result: 

Successfully installed OpenStack and accessed the Horizon Dashboard.


