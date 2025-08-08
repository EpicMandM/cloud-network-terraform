# Cloud Network Terraform

Reusable Terraform configuration for provisioning cloud networking primitives (e.g., virtual networks, subnets, routing, and security rules).

## Prerequisites
- Terraform >= 1.4 (recommended: latest)
- Cloud provider credentials configured in your environment
- Optional: a backend configured for remote state

## Example variables
Create a tfvars file (e.g., example.tfvars) with values appropriate for your environment:
```hcl
region              = "us-east-1"
network_cidr        = "10.0.0.0/16"
public_subnet_cidrs = ["10.0.1.0/24", "10.0.2.0/24"]
private_subnet_cidrs= ["10.0.11.0/24", "10.0.12.0/24"]
tags = {
  project = "cloud-network-terraform"
  env     = "dev"
}
```
