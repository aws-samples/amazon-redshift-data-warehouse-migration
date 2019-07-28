# Verify the Source Data Warehouse before Migration

For the purpose of this workshop, we have used an Amazon RDS for Oracle instance to host the Oracle Data Warehouse. In a real-life situation, this Oracle data warehouse could be on-premises, on Amazon EC2 or on Amazon RDS itself.

Once the CloudFormation Stack is created, an Amazon RDS instance will be provisioned along with the proper security group, DB instance type, storage type configuration and size as specified in the CloudFormation template.

NOTE: To keep things simple for this lab, we have kept most of the configuration static in the CloudFormation template.

This Amazon RDS instance is pre-loaded with a sample schema (dms_sample). The sample schema mimics a simple sporting event ticketing application. The following diagram illustrates the data model we will be working in the lab.

![CloudFormation](img/lab2-image1.png)
voya
