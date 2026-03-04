# TASK 27 - IAM + RBAC + Least Privilege (AWS + Azure)

# Objective
To implement Role-Based Access Control (RBAC) and enforce least privilege access in AWS and Azure.

# Services Used
- AWS IAM
- Azure Entra ID (RBAC)

# AWS Implementation
- Created IAM User (Developer)
- Attached EC2 Full Access Policy
- Created Custom Policy (Deny S3 Delete)
- Attached Policy via IAM Role
- Tested permissions
- Expected Result:
- EC2 access allowed
- S3 delete operation denied

# Azure Implementation
- Created User in Entra ID
- Assigned Reader Role on Resource Group
- Assigned Contributor Role on Specific VM
- Verified restricted access

# Validation
- Confirmed least privilege principle
- Demonstrated allowed & denied actions
 
# Screenshots Included
- IAM policy
- IAM role attachment
- Azure role assignments
