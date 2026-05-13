# /day4-flow-builder/

# README.md

## 1. What is Flow Builder?

Flow Builder is a Salesforce automation tool used to automate business processes without writing code. It helps users create workflows, collect data, update records, send emails, and perform actions automatically using a visual interface.

Flow Builder improves productivity, reduces manual work, and ensures consistent business operations.

---

# 2. Types of Flows

Salesforce provides different types of flows for different automation needs.

## Screen Flow

Screen Flow is an interactive flow that displays screens to users and collects input from them.

### Features
- User interaction
- Forms and screens
- Data collection
- Guided processes

### Example
A customer support form where users enter issue details and submit a request.

---

## Record Triggered Flow

Record Triggered Flow runs automatically when a Salesforce record is created, updated, or deleted.

### Features
- Automatic execution
- No user interaction required
- Updates records automatically
- Sends notifications and emails

### Example
When a new Lead is created, automatically assign it to the sales team.

---

# 3. Your Automation Ideas

## 1. Automatic Lead Assignment
Assign new leads automatically to sales representatives based on region.

## 2. Employee Onboarding Process
Automatically create tasks, emails, and reminders for new employee onboarding.

## 3. Customer Support Ticket Routing
Route customer issues automatically to the correct support team.

## 4. Payment Reminder Notifications
Send reminder emails before invoice due dates.

## 5. Student Attendance Alert
Notify parents automatically when student attendance is low.

---

# 4. Your Flow Diagram

## Example Flow Diagram

```text
Start
  ↓
Get Customer Record
  ↓
Check Payment Due Date
  ↓
Send Reminder Email
  ↓
Update Status
  ↓
End
