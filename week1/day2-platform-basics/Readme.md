# Day 2 – Salesforce Platform Basics

## What is Salesforce Platform?

Salesforce Platform is a cloud-based platform used to build CRM applications, manage customer data, automate workflows, and improve business processes.

It helps companies:

- Store and manage customer data
- Build custom applications
- Automate business operations
- Improve communication between teams
- Increase productivity
- Provide better customer support

Salesforce is highly scalable and can be used by businesses of all sizes.

--------------------------------------------------

# Why Salesforce Platform is Important

Companies use Salesforce Platform because it helps them:

- Manage all customer information in one place
- Create business applications quickly
- Automate repetitive tasks
- Improve collaboration between departments
- Access data from anywhere using the cloud
- Customize applications based on business needs

Salesforce provides both:
- Configuration tools (clicks)
- Development tools (coding)

--------------------------------------------------

# Salesforce Platform Core Concepts

# App

An App in Salesforce is a collection of related tools, objects, tabs, and features used for a specific business purpose.

It acts like a workspace where users can access all related functionality in one place.

Example:
Hospital Management App may include:
- Patients
- Doctors
- Appointments
- Billing

Apps help businesses:
- Organize features properly
- Improve navigation
- Increase user productivity

--------------------------------------------------

# Object

An Object is like a database table used to store specific business information.

Objects contain:
- Records (rows)
- Fields (columns)

Types of Objects:

1. Standard Objects
Objects already provided by Salesforce:
- Account
- Contact
- Opportunity
- Lead

2. Custom Objects
Objects created based on business requirements:
- Student
- Patient
- Library Book
- Attendance

Example:
A Student Object may store:
- Student Name
- Roll Number
- Department
- Email

Objects help businesses organize and manage data efficiently.

--------------------------------------------------

# Tab

A Tab is a navigation tool used to access Objects, Apps, Dashboards, and Pages in Salesforce.

Tabs help users open and manage records easily.

Example:
Contacts Tab allows users to:
- View contacts
- Create new contacts
- Edit contact details

Tabs improve:
- Navigation
- Accessibility
- User experience

--------------------------------------------------

# Salesforce Architecture

# Multi-Tenant Architecture

Salesforce follows a Multi-Tenant Architecture.

This means multiple companies use the same Salesforce infrastructure securely while keeping their data separate.

Advantages:
- Low maintenance cost
- Automatic updates
- High security
- Better scalability

Real-Life Example:
Like many families living in one apartment building:
- Same building
- Separate apartments

Similarly:
- Same Salesforce servers
- Separate company data

--------------------------------------------------

# Difference Between Configuration and Coding

# Configuration (No Code)

Configuration means creating features using clicks instead of programming.

Salesforce provides tools that allow admins to customize applications without writing code.

When to Use Configuration:
- Requirements are simple
- Built-in Salesforce features are enough
- Fast implementation is needed

Examples:
- Validation Rules
- Workflow Automation
- Creating Fields
- Page Layout Customization

Advantages:
- Faster development
- Easy maintenance
- No coding knowledge needed

--------------------------------------------------

# Coding (Apex)

Coding means writing custom logic using Apex, Lightning Components, APIs, or Triggers.

Developers use coding when business requirements are complex.

When to Use Coding:
- Advanced business logic is required
- External system integration is needed
- Configuration cannot solve the problem

Examples:
- Payment gateway integration
- Complex approval process
- Advanced calculations
- Custom automation

Advantages:
- Highly flexible
- Supports advanced functionality
- Allows deep customization

--------------------------------------------------

# Core Task 1: Connect CRM Concepts with Salesforce Platform

CRM concepts fit into Salesforce using Objects and Apps.

| CRM Concept | Salesforce Representation |
|-------------|--------------------------|
| Account     | Object                   |
| Contact     | Object                   |
| Opportunity | Object                   |

These objects work together inside Salesforce Apps.

Business Flow:

Lead → Contact → Opportunity → Customer

Explanation:

1. Lead
A Lead is a person who shows interest in a product or service but is not yet confirmed as a customer.

Examples:
- Website inquiry
- Registration form submission

--------------------------------------------------

2. Contact
After verification, the Lead becomes a Contact.

A Contact stores:
- Name
- Phone Number
- Email
- Customer Details

--------------------------------------------------

3. Opportunity
An Opportunity represents a possible business deal.

It helps companies track:
- Deal amount
- Sales stage
- Revenue
- Closing date

--------------------------------------------------

4. Customer
When the deal is completed successfully, the person becomes a Customer.

This process helps businesses manage sales efficiently.

--------------------------------------------------

# Core Task 2: Platform Understanding

# What is an App?

An App is a collection of related tools, tabs, and objects designed for a business process.

Example:
College Management App

Contains:
- Students
- Faculty
- Courses
- Attendance

--------------------------------------------------

# What is an Object?

An Object is a database table used to store data.

Example:
Student Object stores:
- Student Name
- Roll Number
- Department

--------------------------------------------------

# What is a Tab?

A Tab helps users access objects and records easily.

Example:
Students Tab opens all student records.

--------------------------------------------------

# Core Task 3: Configuration vs Coding

# Configuration Examples

Example 1:
Validation Rule:
Prevent users from saving records without Email.

Example 2:
Workflow Automation:
Automatically send email after record creation.

--------------------------------------------------

# Coding Examples

Example 1:
Integrating Salesforce with Payment Gateway.

Example 2:
Creating complex calculations using Apex Trigger.

--------------------------------------------------

# Core Task 4: Real-Life System Design

# Example: College Management System

App Name:
College Management App

--------------------------------------------------

Objects Inside the App

Standard Objects:
- Contact
- Account

Custom Objects:
- Student
- Faculty
- Course
- Attendance
- Examination

--------------------------------------------------

# User Interaction

Students Can:
- View attendance
- Check results
- Access courses

Faculty Can:
- Update attendance
- Add marks
- Manage subjects

Admin Can:
- Manage records
- Generate reports
- Assign faculty

--------------------------------------------------

#  Must Include

1. What is Salesforce Platform?

Explain:
- Salesforce overview
- Cloud platform
- CRM capabilities
- Automation and customization

--------------------------------------------------

2. Explain

App:
Collection of related tools and objects.

Object:
Database table used to store information.

Tab:
Navigation tool used to access records.

--------------------------------------------------

3. Difference Between Configuration vs Coding

| Configuration       | Coding                    |
|---------------------|---------------------------|
| Uses clicks         | Uses programming          |
| Simple customization| Advanced customization    |
| Faster              | More flexible             |
| No coding required  | Requires development knowledge |

--------------------------------------------------

4. Your System Design

App Name:
College Management App

Objects:
- Student
- Faculty
- Attendance
- Course
- Examination

User Interaction:
Students, faculty, and admins interact with records using tabs and apps.

--------------------------------------------------

5. Screenshots from Trailhead

Add screenshots of:
-  Agentforce 360 Platform Basics
- Agentforce 360 Platform Development Basic

--------------------------------------------------
Using:
- Apex
- APIs
- Lightning Components
- Triggers
- Integrations
