# Implementing VPC Peering on AWS


## Objective

This project aimed to implement VPC peering between two Virtual Private Clouds (VPCs) on AWS to enable communication between instances in different VPCs. The goal was to securely connect resources in separate VPCs without requiring them to communicate over the public internet. This project demonstrates intermediate-level skills in AWS VPC management, EC2 instance configuration, and RDS database setup.

### Skills Learned

- VPC Configuration: Creating and managing VPCs and their associated subnets, route tables, and internet gateways.
- VPC Peering: Establishing VPC peering connections to enable communication between resources in different VPCs.
- EC2 Management: Launching and configuring EC2 instances within VPCs.
- RDS Setup: Creating and managing RDS instances and configuring security groups for secure database access.
- Network Configuration: Setting up route tables and security groups to allow secure and efficient traffic routing between peered VPCs.

### Tools Used

- Amazon EC2: For launching and managing virtual machines.
- Amazon VPC: For creating and managing VPCs and related networking components.
- Amazon RDS: For setting up and managing relational databases.
- AWS Management Console: For configuring and managing all AWS resources.


### Outcome
The project successfully demonstrated the implementation of VPC peering between two VPCs, allowing secure communication between resources in different VPCs. By completing this project, I have showcased the ability to effectively manage AWS networking resources and configure secure communication channels between isolated networks.

## Steps

Create 2 VPCs in same region 

<img width="1468" alt="Screenshot 2024-05-14 at 1 07 37 PM" src="https://github.com/Hunter102002/implement-VPC-Peering/assets/98543129/de75233e-af0c-4dfd-9aab-8447e531bb28">

<img width="1470" alt="Screenshot 2024-05-14 at 1 08 21 PM" src="https://github.com/Hunter102002/implement-VPC-Peering/assets/98543129/e9771795-36d8-46ea-b8c6-a99022ae0b95">

Create and attatch Internet Gateway

<img width="1470" alt="Screenshot 2024-05-14 at 1 09 01 PM" src="https://github.com/Hunter102002/implement-VPC-Peering/assets/98543129/423f4993-7874-4a6c-a177-0536188a39ac">


<img width="1470" alt="Screenshot 2024-05-14 at 1 09 28 PM" src="https://github.com/Hunter102002/implement-VPC-Peering/assets/98543129/ea28cacb-37c0-46c6-83df-a599328cc779">

Create 2 Subnets for VPC1

<img width="1190" alt="Screenshot 2024-05-14 at 1 11 32 PM" src="https://github.com/Hunter102002/implement-VPC-Peering/assets/98543129/81c00b7a-b5b2-458f-b03f-4bdffc30eae4">

Create 2 Subnets for VPC2

<img width="1191" alt="Screenshot 2024-05-14 at 1 13 21 PM" src="https://github.com/Hunter102002/implement-VPC-Peering/assets/98543129/db2f24a2-d5d4-413a-82c6-8367c715631b">

Attach the 2 subnets to each of the VPCs


<img width="1470" alt="Screenshot 2024-05-14 at 1 14 41 PM" src="https://github.com/Hunter102002/implement-VPC-Peering/assets/98543129/b610675d-fb39-4b5d-8c75-611a82a5679a">


<img width="1439" alt="Screenshot 2024-05-14 at 1 15 24 PM" src="https://github.com/Hunter102002/implement-VPC-Peering/assets/98543129/ae0781eb-53fe-42cd-aed9-f96438e5caf6">

Edit the route tables

<img width="1424" alt="Screenshot 2024-05-14 at 1 16 31 PM" src="https://github.com/Hunter102002/implement-VPC-Peering/assets/98543129/91e5f15d-7d8e-49ea-8e4b-f0a398fa46f0">

Request and Accept for VPC Peering

<img width="1464" alt="Screenshot 2024-05-14 at 1 19 27 PM" src="https://github.com/Hunter102002/implement-VPC-Peering/assets/98543129/327e2b18-2652-4814-960a-ec308b2fc0f1">


<img width="818" alt="Screenshot 2024-05-14 at 1 22 37 PM" src="https://github.com/Hunter102002/implement-VPC-Peering/assets/98543129/f4726f23-9799-41f0-8a94-1fb57b87d435">

Edit Routes in route tables

<img width="1143" alt="Screenshot 2024-05-14 at 1 24 19 PM" src="https://github.com/Hunter102002/implement-VPC-Peering/assets/98543129/340f6d13-5473-4ab6-b2d4-9169c39ec3b2">

<img width="1143" alt="Screenshot 2024-05-14 at 1 25 04 PM" src="https://github.com/Hunter102002/implement-VPC-Peering/assets/98543129/93949a46-ccf9-46e5-b63c-8fd3e7837779">

Create EC2 Instance

<img width="1449" alt="Screenshot 2024-05-14 at 1 31 44 PM" src="https://github.com/Hunter102002/implement-VPC-Peering/assets/98543129/29d2c061-1633-4214-b09a-cde0034e63a9">

Create Security group for RDS instance

<img width="1446" alt="Screenshot 2024-05-14 at 1 34 17 PM" src="https://github.com/Hunter102002/implement-VPC-Peering/assets/98543129/2cd82949-c046-44d7-9785-2fae6ff52d3a">

Create the RDS database

<img width="1072" alt="Screenshot 2024-05-14 at 1 39 41 PM" src="https://github.com/Hunter102002/implement-VPC-Peering/assets/98543129/552e2dce-d07e-43ab-a461-e686426a71eb">

SSH into database and verify connection


<img width="895" alt="Screenshot 2024-05-14 at 1 48 55 PM" src="https://github.com/Hunter102002/implement-VPC-Peering/assets/98543129/35720a81-935a-4c28-bbcf-d7bebdced26d">
