# AWS Identity and Access Managment - Role-Based Access Control (RBAC) 

## Overview
This project demonstrates a role-based IAM architecture in AWS designed around least-privilege priciples. The goal is to model how different user personas (Admin, Developer, Read-only Analyat) are secuirely authorized to access cloud resources.

This mirrors real-world identity governance and access management (IAM/IGA) scenarios used in enterprise enviorments.

---

## Architecture Summary 
- AWS Account with IAM enabled
- IAM Users assigned to Groups
- Custom IAM Policies written in JSON
- Permissions scoped to EC2, S3, and CloudWatch 

## User Roles 
| Role | Purpose| 
|------|--------|
| Admin | Full access for cloud administration |
| Developer | Limited access for application deployment | 
| Read-Only Analyst | Visibility without modification rights | 

---

## Implemenation Steps 
1. Created IAM users for each role
2. Created IAM groups matching role definitions
3. Wrote custom IAM policies using JSON
4. Attached policies to groups
5. Validated access via login and permission testing

---

## Secuirty Design 
- Enforced least-privilege access
- Avodied wildcard permissions
- Scoped permissions by service and action

  ---

## Validation
  Each user was tested to confirm:
- Admin can create and manage EC2
- Developer can start/ stop EC2 but cannot modify IAM
- Read-only user can view resources but cannot make changes

---

## Screenshots 


  
