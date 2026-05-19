# gcp-secure-network-segmentation
Designed and implemented a secure enterprise-style network architecture on Google Cloud Platform using custom VPC networking, public/private subnet segmentation, firewall security rules, Compute Engine virtual machines, and internal-only workload communication.
# Secure Public-Private Network Architecture on GCP

## Project Overview

This project demonstrates the implementation of a secure enterprise-style networking architecture on Google Cloud Platform using custom VPC networking, public/private subnet segmentation, firewall security rules, and Compute Engine virtual machines.

The architecture separates internet-facing workloads from internal-only workloads using subnet isolation and controlled internal communication.

---

## Objectives

* Design custom VPC architecture
* Implement public and private subnet segmentation
* Configure firewall-based traffic control
* Deploy public and private workloads
* Validate internal VM communication using private IPs

---

## Services Used

| Service             | Purpose                       |
| ------------------- | ----------------------------- |
| VPC Network         | Enterprise network isolation  |
| Subnets             | Workload segmentation         |
| Firewall Rules      | Traffic control and security  |
| Compute Engine      | VM deployment                 |
| Internal Networking | Secure workload communication |

---

## Architecture Design

secure-vpc

* public-subnet → public-vm
* private-subnet → private-vm

The public VM is internet-accessible while the private VM is accessible only internally through private IP communication.

---

## Key Learnings

* Difference between public and private workloads
* Importance of subnet segmentation
* Internal vs external IP communication
* Firewall-controlled internal communication
* Enterprise security architecture principles

---

## Internal Connectivity Validation

The public VM successfully communicated with the private VM using the private internal IP address (10.10.2.2), validating internal VPC routing and firewall configuration.

---

## Future Improvements

* Add Cloud NAT
* Configure Load Balancer
* Implement Managed Instance Groups
* Add Cloud Armor
* Enable Monitoring and Logging
* Deploy infrastructure using Terraform
