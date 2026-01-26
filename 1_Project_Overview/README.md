# Project Overview – HyGo College RBSMS

## Background

HyGo College RBSMS (Role-Based School Management System) was developed as my postgraduate capstone project aimed at improving administrative efficiency, transparency, and
communication in educational institutions.

The system was designed to address common challenges in schools such as:

- Manual attendance tracking  
- Inefficient grading workflows  
- Limited parent–teacher communication  
- Poor visibility into academic performance  

The solution introduces a centralized, role-based digital platform tailored for resource-constrained school environments.

## Project Objectives

The key objectives of this project were to:

- Design role-based portals for administrators, teachers, and parents  
- Implement secure authentication and role-based access control  
- Automate core academic processes:
  - Attendance tracking  
  - Grading & result management  
  - Performance reporting  
- Introduce geofenced staff attendance using GPS verification  
- Enable real-time communication between stakeholders  
- Ensure mobile responsiveness and accessibility  

## User Roles & Capabilities

### Administrator

Key responsibilities:

- Manage all user accounts  
- View institutional metrics and reports  
- Approve grades  
- Configure geofencing boundaries  
- Monitor staff attendance  
- Broadcast announcements  

### Teacher

Key responsibilities:

- GPS-verified clock-in and clock-out  
- Record student attendance  
- Submit grades with validation  
- Generate performance reports  
- Message parents and administrators  
- View class rosters  

### Parent

Key responsibilities:

- View children’s grades  
- Access attendance history  
- Download report cards  
- Receive absence and performance notifications  
- Communicate with teachers  

## System Architecture

- **Frontend:** React (Vite)  
- **Backend:** Spring Boot (REST APIs)  
- **Database:** MySQL  

The system follows a layered architecture:

- Presentation Layer (React UI)  
- Application Layer (Spring Boot services)  
- Data Layer (MySQL)  

Role-based access is enforced at both API and UI levels.

## QA Involvement

As both developer and QA engineer, I:

- Derived test conditions directly from user stories and acceptance criteria  
- Designed functional and negative test scenarios  
- Executed manual test cycles across all major modules  
- Logged and tracked defects  
- Performed regression testing after fixes  
- Produced professional QA documentation  

This dual role provided deep insight into both **system design** and **system quality**.

## QA Artefacts Included in This Repository

This repository contains curated samples of:

- Requirements summaries  
- Test plan  
- Sample test cases  
- Sample bug reports  
- Test summary & closure report  

These artefacts represent industry-style QA documentation applied to a real system.
