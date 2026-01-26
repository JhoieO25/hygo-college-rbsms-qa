# User Roles & Key Features – HyGo College RBSMS

This document summarizes the primary user roles and core system capabilities derived from the project’s Business Requirements and User Stories.

## 1. Administrator

**Primary Responsibilities**

- Manage all user accounts (create, update, deactivate)
- View institutional metrics and dashboards
- Approve and publish grades
- Configure geofencing boundaries for staff attendance
- Monitor staff clock-in and clock-out records
- Broadcast announcements to teachers and parents

**Key Features Tested**

- Role-based access control (admin-only actions)
- User management workflows
- Grade approval validation
- Geofence configuration and enforcement

## 2. Teacher

**Primary Responsibilities**

- GPS-verified clock-in and clock-out
- Record student attendance
- Submit grades with validation rules
- View assigned class roosters
- Message administrators

**Key Features Tested**

- Attendance capture and editing
- Grade submission validation
- Access restrictions by class ownership
- Performance report generation
- Messaging workflows

## 3. Parent

**Primary Responsibilities**

- View children’s grades
- Access attendance history
- Communicate with administrator

**Key Features Tested**

- Read-only access to child records
- Data privacy between parents

## Notes on QA Usage

These roles and features were used as the foundation for:

- Test scenario design  
- Functional and negative test cases  
- Access control validation  
- End-to-end user journey testing  

Only high-level role summaries are included here.
