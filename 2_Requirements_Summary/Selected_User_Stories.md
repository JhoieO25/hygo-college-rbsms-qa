# Selected User Stories – HyGo College RBSMS

This document contains a curated selection of user stories extracted from the full requirements specification.

These stories were used directly to design functional and validation test cases.

## Authentication & Access Control

### US-01: Administrator Login

**As an** Administrator  
**I want to** log into the system securely  
**So that** I can manage users and institutional data  

**Acceptance Criteria**

- Login succeeds with valid credentials  
- Login fails with invalid credentials  
- Unauthorized users cannot access admin features  

### US-02: Role-Based Access Restriction

**As a** User  
**I want to** only see features assigned to my role  
**So that** I cannot access unauthorized functions  

**Acceptance Criteria**

- Admin features are hidden from teachers and parents  
- Teachers cannot access admin dashboards  
- Parents cannot access grading modules  

## Attendance Management

### US-03: Teacher Clock-In with GPS Verification

**As a** Teacher  
**I want to** clock in only when inside the approved geofence  
**So that** attendance records are accurate  

**Acceptance Criteria**

- Clock-in allowed within geofence boundary  
- Clock-in blocked outside boundary  
- System records timestamp and location  

### US-04: Record Student Attendance

**As a** Teacher  
**I want to** mark student attendance for my class  
**So that** attendance records are accurate and auditable  

**Acceptance Criteria**

- Only assigned classes are visible  
- Attendance cannot be submitted with missing students  
- Changes are logged  

## Grading & Reporting

### US-05: Parent Views Report Card

**As a** Parent  
**I want to** view my child’s school report  
**So that** I can review academic performance in real time.

**Acceptance Criteria**

- Only own child’s data visible  
- Data matches stored grades  

## Notes on Usage

These user stories were directly mapped to:

- Functional test scenarios  
- Validation test cases  
- Negative and boundary testing  

Only a subset is shown here to demonstrate test design quality without exposing full academic documentation.
