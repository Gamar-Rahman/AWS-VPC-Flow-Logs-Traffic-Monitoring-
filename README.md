# AWS-VPC-Flow-Logs-Traffic-Monitoring-
Hands-on AWS lab focused on building a VPC, configuring networking components, enabling VPC Flow Logs, generating traffic, and analyzing network activity for monitoring and security visibility.
# AWS VPC Flow Logs and Traffic Monitoring Lab

## Overview
This lab demonstrates how to create an Amazon VPC, configure its networking components, and enable VPC Flow Logs to capture and analyze network traffic. It also includes generating traffic to observe how network activity is recorded for monitoring, troubleshooting, and security analysis.

This project is valuable for anyone learning cloud networking, AWS security, and network visibility in cloud environments.

## Lab Title
Creating AWS VPC Flow Logs and Generating Traffic

## Objective
The goal of this lab is to understand how to:
- Create and configure an Amazon VPC
- Set up subnets, route tables, and an internet gateway
- Launch resources inside the VPC
- Enable VPC Flow Logs
- Generate network traffic
- Review and analyze captured traffic logs

## Why This Lab Matters
Amazon VPC is the foundation of secure cloud networking in AWS. VPC Flow Logs provide visibility into network traffic entering and leaving network interfaces within your VPC. This is important for:
- Network troubleshooting
- Traffic analysis
- Incident investigation
- Threat detection
- Security monitoring
- Compliance and auditing

From a cybersecurity perspective, VPC Flow Logs help identify suspicious behavior such as unauthorized connections, scanning activity, denied traffic, and unusual communication patterns.

## AWS Services Used
- Amazon VPC
- VPC Subnets
- Route Tables
- Internet Gateway
- EC2
- VPC Flow Logs
- CloudWatch Logs

## Architecture
The environment includes:
- One custom Amazon VPC
- Public subnet
- Internet Gateway
- Route table for internet access
- EC2 instance inside the subnet
- VPC Flow Logs sending traffic metadata to CloudWatch Logs

## Lab Steps
1. Create a custom Amazon VPC
2. Create a subnet inside the VPC
3. Attach an Internet Gateway to the VPC
4. Configure the route table for internet access
5. Launch an EC2 instance in the subnet
6. Enable VPC Flow Logs for the VPC
7. Send flow logs to CloudWatch Logs
8. Generate traffic from the instance
9. Review the logs and observe accepted or rejected traffic patterns

## Key Concepts Learned

### 1. Amazon VPC
Amazon VPC allows you to create a logically isolated network in AWS. You define IP ranges, subnets, gateways, and routing behavior.

### 2. Subnets
Subnets divide the VPC into smaller network segments. Public subnets allow internet-connected resources, while private subnets are used for internal systems.

### 3. Internet Gateway
An Internet Gateway allows communication between your VPC and the internet.

### 4. Route Tables
Route tables define where network traffic is directed. For a public subnet, a route to the Internet Gateway is required.

### 5. VPC Flow Logs
VPC Flow Logs capture metadata about network traffic such as:
- Source IP
- Destination IP
- Source port
- Destination port
- Protocol
- Number of packets
- Bytes transferred
- Action taken (ACCEPT or REJECT)

## Security Relevance
This lab directly supports cloud security learning by demonstrating how to:
- Monitor east-west and north-south traffic
- Investigate allowed and denied network communications
- Detect anomalies in traffic behavior
- Support incident response and threat hunting in AWS

VPC Flow Logs are especially useful in identifying:
- Unauthorized access attempts
- Suspicious outbound traffic
- Misconfigured security groups or NACLs
- Unexpected communication between workloads

## Example Use Cases
- Investigating unusual traffic in a cloud network
- Troubleshooting connectivity between subnets
- Validating security group rules
- Supporting forensic review after a security event
- Monitoring traffic patterns for compliance

## Skills Demonstrated
- AWS networking fundamentals
- Cloud security monitoring
- Log analysis
- Traffic visibility in AWS
- VPC design and configuration
- Security-focused cloud operations

## Project Outcome
By completing this lab, I gained practical experience in creating a secure AWS network, enabling traffic visibility, and understanding how network logs can support both operational troubleshooting and cybersecurity investigations.

## Future Improvements
Possible next steps for expanding this lab:
- Send VPC Flow Logs to Amazon S3 for long-term retention
- Analyze logs with Athena
- Build dashboards in CloudWatch
- Detect anomalies with automation
- Integrate with GuardDuty for threat detection
- Create alerts for suspicious traffic patterns

