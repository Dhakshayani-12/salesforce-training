Day 2  – Salesforce Platform Basics

1. Salesforce Platform Basics

You learn:

Platform overview
Navigation inside Salesforce
Apps and Objects
Platform structure
Important Concepts
Salesforce is cloud-based
Data is organized using Objects
Apps combine related features together
Tabs help users navigate
2. Salesforce Development Basics

You learn:

How development happens in Salesforce
Difference between Admin work and Developer work
Configuration vs Coding
Introduction to:
Apex
APIs
UI Customization
3. Salesforce Architecture

You understand:

Multi-tenant architecture
How Salesforce serves multiple companies securely
Why Salesforce is scalable and efficient
Multi-Tenant Example

Like many families living in one apartment building:

Same building
Separate apartments

Similarly:

Same Salesforce infrastructure
Separate customer data

CORE TASKS
Task 1 – Connect Day 1 + Day 2

Explain: 
� How CRM concepts (Account, Contact, Opportunity) 
fit into Salesforce Platform (Objects, Apps)

Explanation

CRM concepts like:

Account
Contact
Opportunity

are implemented in Salesforce using Objects.

CRM Concept	Salesforce Representation
Account	Object
Contact	Object
Opportunity	Object

These objects are grouped inside an App such as the Sales App.

Example Flow
Company information stored in Account
Customer details stored in Contact
Sales deals stored in Opportunity

This structure helps businesses manage customer relationships efficiently.

Task 2 – Platform Understanding
1. What is an App in Salesforce?

An App is a collection of related tools, objects, tabs, and features designed for a specific business process.

Example

Hospital Management App may include:

Patients
Doctors
Appointments
Billing
Purpose
Organizes work
Improves navigation
Provides one workspace for users

2. What is an Object?

An Object is like a database table used to store information.

Objects contain:

Records (rows)
Fields (columns)
Types of Objects
Standard Objects

Built-in Salesforce objects:

Account
Contact
Opportunity
Custom Objects

Created by users/developers:

Student
Patient
Library Book
Example

Student Object may contain:

Student Name
Roll Number
Email
3. What is a Tab?

A Tab is used to access objects, apps, dashboards, or pages in Salesforce.

Example

Contacts Tab opens:

Contact records
Create new contact option
Edit contact option
Purpose
Easy navigation
Quick access to data

Task 3 – Configuration vs Coding
Configuration (No Code)

Configuration means building features using clicks instead of programming.

When to Use

Use configuration when requirements are simple.

Examples
Validation Rules
Workflow Automation
Creating Fields
Page Layout Changes
Advantages
Faster
Easier maintenance
No coding needed
Coding (Apex)

Coding means writing custom logic using Apex or Lightning Components.

When to Use

Use coding for complex business requirements.

Examples
External system integration
Complex approval processes
Advanced calculations
Custom business logic
Advantages
More flexibility
Supports complex features
Highly customizable
Task 4 – Real System Thinking
Example System: College Management System
App Name

College Management App

Objects Inside the App
Standard Objects:
Contact
Account
Custom Objects:
Student
Faculty
Course
Attendance
Examination
User Interaction
Students Can:
View attendance
Check marks
View courses
Faculty Can:
Update attendance
Add marks
Manage courses
Admin Can:
Manage records
Generate reports
Assign faculty
