# Initial Setup for CloudCorpConfigurator

Welcome to the first step of setting up your robust corporate network on AWS with `CloudCorpConfigurator`. This guide will introduce you to the initial steps and prerequisites for deploying a seamless, secure, and scalable AWS corporate network. Even if you have minimal IT knowledge, by the end of this guide, you should have a foundational understanding of what we'll be building and the initial preparations.

## Table of Contents

1. [Prerequisites](#prerequisites)
2. [AWS Account Setup](#aws-account-setup)
3. [IAM Users and Permissions](#iam-users-and-permissions)
4. [Regions and Availability Zones](#regions-and-availability-zones)
5. [Cost Management](#cost-management)
6. [Next Steps](#next-steps)

## Prerequisites

Before diving in, make sure you have:

- An active AWS account. If not, [sign up here](https://aws.amazon.com/).
- A computer with internet connectivity.
- Basic familiarity with AWS services. If not, consider skimming through the [AWS basics documentation](https://aws.amazon.com/getting-started/tutorials/).

## AWS Account Setup

1. **Sign in**: Log into the [AWS Management Console](https://aws.amazon.com/console/).
2. **Billing**: Ensure that your billing information is correctly set up. AWS services can incur costs.
3. **Support Plan**: Consider choosing a support plan if you anticipate needing AWS support or guidance.

## IAM Users and Permissions

Never use the root user for regular tasks. Instead:

1. Navigate to **IAM** in the AWS Management Console.
2. Create a new user with programmatic and console access. This will be the user you use for most tasks.
3. Assign policies based on the principle of least privilege. For this guide, `AdministratorAccess` might be useful, but in production, permissions should be more restrictive.

## Regions and Availability Zones

AWS has various global regions. Each region has multiple Availability Zones (data centers). 

1. Choose a region close to your major user base for optimal performance. For instance, if most users are in Europe, consider `eu-central-1` (Frankfurt).
2. Plan to distribute resources across Availability Zones for high availability.

## Cost Management

1. AWS can cost money, so always keep an eye on the AWS Cost Explorer.
2. Set up a billing alarm to be notified if your costs exceed a particular amount.
3. Consider using the AWS Free Tier if you are just testing things out, but be aware of its limits.

## Next Steps

With the initial setup complete, you're now ready to dive deep into building your corporate network infrastructure. Navigate to the `02-vpc-setup.md` for a step-by-step guide on creating your VPC.

---

Thank you for choosing `CloudCorpConfigurator`! Together, we'll build a resilient, secure, and optimized corporate network on AWS.
