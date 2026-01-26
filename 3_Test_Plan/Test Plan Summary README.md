# Test Plan – HyGo College Role-Based School Management System (RBSMS)

## 1. Introduction

This test plan describes the overall testing strategy, scope, approach, and responsibilities for the Quality Assurance activities carried out on the
HyGo College Role-Based School Management System (RBSMS).

The objective of testing was to ensure that the system meets functional, security, usability, and reliability requirements before production deployment.

## 2. Test Objectives

The primary objectives of testing were to:

- Validate that core academic and administrative workflows function correctly  
- Verify role-based access control for all user roles  
- Ensure data accuracy for attendance, grading, and reporting  
- Validate system behavior under network constraints  
- Identify and document functional and usability defects  

## 3. Scope of Testing

### In Scope

The following modules and features were tested:

- Authentication and role-based access control  
- Administrator portal  
- Teacher portal  
- Parent portal  
- Attendance management  
- Grade submission and approval  
- Report generation and downloads  
- Messaging and notifications  
- Geofenced staff clock-in/clock-out  
- Basic API endpoints supporting core workflows  

### Out of Scope

The following were not covered in this test cycle:

- Third-party payment integrations  
- Production deployment monitoring  
- Load testing at enterprise scale  
- External system integrations not implemented in this project  

## 4. Test Approach & Strategy

Testing was conducted using a combination of:

- Requirement-based testing  
- Functional black-box testing  
- Positive and negative test scenarios  
- Boundary value testing  
- Exploratory testing  

Test design was derived directly from:

- Business Requirements Document (BRD)  
- User Stories and Acceptance Criteria  
- System architecture and role definitions  

## 5. Types of Testing Performed

The following test types were executed:

- Functional Testing  
- Integration Testing  
- User Interface (UI) Testing  
- Access Control & Security Testing  
- Network Condition Testing (offline and throttled network)  
- Regression Testing  
- User Acceptance Testing (UAT – simulated)  

## 6. Test Environment

- Frontend: React (Vite)  
- Backend: Spring Boot  
- Database: MySQL  
- Browser: Google Chrome  
- Operating System: Windows 10  
- Network Simulation: Chrome DevTools (Offline / Throttled Network)  

## 7. Test Data

Test data included:

- Sample administrator, teacher, and parent accounts  
- Multiple class and subject configurations  
- Valid and invalid grade values  
- Valid and invalid attendance records  

All test data was anonymized and created solely for testing purposes.

## 8. Entry Criteria

Testing commenced when:

- Core features were implemented and deployable locally  
- User roles and access control were configured  
- Database schema was stable 

## 9. Exit Criteria

Testing was considered complete when:

- All high-priority test cases were executed  
- Critical defects were fixed or documented  
- Test summary and closure report were produced  
- No open critical or blocker defects remained

## 10. Defect Management

Defects were:

- Logged with severity and priority  
- Documented with reproduction steps and evidence  
- Tracked through resolution and verification  

## 11. Risks & Mitigation

| Risk | Mitigation |
|-----|-----------|
| Authorization & access control issues | Test each role extensively |
| Data inconsistency | Validation and reconciliation checks |
| Network instability | Offline and throttled network testing |
| Single-developer bias | Structured test design and independent verification |

## 12. Deliverables

The following QA deliverables were produced:

- Test Plan  
- Test Scenarios  
- Test Cases  
- Bug Reports  
- Test Summary & Closure Report  
- Sample Evidence (screenshots & logs)  

## 13. Conclusion

This test plan demonstrates a structured QA approach applied to a real-world academic software system developed and tested end-to-end.

