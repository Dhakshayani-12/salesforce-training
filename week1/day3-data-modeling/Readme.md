# Salesforce Summer Program – Day 3

---

# Key Concepts Learned

## 1. Objects
Objects are database tables used to store data in Salesforce.

### Examples:
- Student
- Faculty
- Course
- Department

---

## 2. Fields
Fields are individual pieces of information stored inside an object.

### Examples:
- Name
- Email
- Age
- Course Name

---

## 3. Records
A record is a single entry inside an object.

### Example:
A single student’s details inside the Student object.

---

# Standard vs Custom Objects

## Standard Objects
These are pre-built objects provided by Salesforce.

### Examples:
- Account
- Contact
- Opportunity

---

## Custom Objects
These are objects created by users based on business requirements.

### Examples:
- Student
- Faculty
- Course

---

# Relationship Types in Salesforce

## One-to-Many Relationship
One record can be connected to many records.

### Example:
- One Department can have many Students.
- One Course can have many Students.

---

## Lookup Relationship
A relationship used to connect two objects.

### Example:
- Student → Course
- Faculty → Department

---

# Why Enterprise Systems Need Structured Data

Structured data helps organizations:
- Store information properly
- Reduce duplicate records
- Improve reporting
- Maintain data accuracy
- Increase productivity
- Improve decision-making

Without structured data, random spreadsheets can create confusion, errors, and missing information.

---

# Formula Fields

Formula fields automatically calculate values using formulas.

### Examples:
- Full Name
- Percentage
- Remaining Seats

### Benefits:
- Saves time
- Reduces manual errors
- Automatically updates values

---

# Validation Rules

Validation rules ensure only correct data is entered into the system.

### Examples:
- Email cannot be blank
- Age cannot be negative
- Course seats cannot exceed limit

### Benefits:
- Prevents bad data
- Maintains data quality
- Improves system reliability



Data Modeling (College Management System)

## 1. Difference Between App, Object, Record, and Field

| Term | Meaning | Example |
|------|----------|----------|
| App | A collection of related tools/features used for a business process | College Management App |
| Object | A table that stores similar types of data | Student Object |
| Record | One single row/data entry inside an object | Student: Ravi Kumar |
| Field | A column that stores one piece of information | Student Name, Email |

---

# 2. Standard vs Custom Objects

## Standard Objects
These are pre-built objects provided by the platform.

### Examples:
- Account
- Contact
- Opportunity

### Features:
- Already available
- Common business usage
- Less customization needed

---

## Custom Objects
These are objects created by users based on business requirements.

### Examples in College System:
- Student
- Faculty
- Course
- Department

### Features:
- Fully customizable
- Designed for specific business needs
- Helps organize custom data

---

# 3. College Management System Data Model

## Objects

### Student
Stores student details.

#### Fields:
- Student ID
- First Name
- Last Name
- Email
- Age
- Course
- Department
- Percentage

---

### Faculty
Stores faculty information.

#### Fields:
- Faculty ID
- Faculty Name
- Email
- Department
- Subject

---

### Course
Stores course details.

#### Fields:
- Course ID
- Course Name
- Total Seats
- Enrolled Students
- Remaining Seats

---

### Department
Stores department information.

#### Fields:
- Department ID
- Department Name
- HOD Name

---

# Relationships

| Relationship | Type | Explanation |
|--------------|------|-------------|
| Department → Students | One-to-Many | One department can have many students |
| Department → Faculty | One-to-Many | One department can have many faculty members |
| Course → Students | One-to-Many | One course can have many students |
| Department → Courses | One-to-Many | One department can offer many courses |

---

# Lookup Relationships

| Object | Lookup To | Reason |
|--------|------------|--------|
| Student | Course | Student belongs to one course |
| Student | Department | Student belongs to one department |
| Faculty | Department | Faculty works in one department |
| Course | Department | Course belongs to one department |

---

# 4. Formula Fields

## 1. Full Name

### Formula:
```text
First Name + " " + Last Name
```

### Explanation:
This field automatically combines the student's first name and last name into a single field.  
It saves time and avoids manual typing mistakes.

---

## 2. Remaining Seats

### Formula:
```text
Total Seats - Enrolled Students
```

### Explanation:
This field automatically calculates how many seats are available in a course.  
It updates whenever a new student enrolls and prevents incorrect seat counts.

---

## 3. Percentage

### Formula:
```text
(Obtained Marks / Total Marks) * 100
```

### Explanation:
This field automatically calculates the student’s percentage based on marks entered.  
It reduces manual calculation errors and ensures accuracy.

---

# 5. Validation Rules

## 1. Email Cannot Be Empty

### Rule:
The Email field should not be blank.

### Prevents:
- Missing communication details
- Incomplete student records

---

## 2. Student Age Cannot Be Negative

### Rule:
Age must be greater than 0.

### Prevents:
- Invalid student information
- Incorrect database records

---

## 3. Enrolled Students Cannot Exceed Total Seats

### Rule:
Enrolled Students <= Total Seats

### Prevents:
- Overbooking courses
- Incorrect seat management

---

# 6. Reflection – Why Structured Enterprise Data Matters

Structured enterprise data is important because it keeps information organized, accurate, and easy to manage. Companies handle large amounts of data every day, and random spreadsheets can create duplicate records, missing information, and confusion.

Structured data helps companies:
- Store data in a proper format
- Improve teamwork between departments
- Generate reports quickly
- Reduce errors
- Maintain consistency
- Make better business decisions

For example, in a college management system, structured data helps manage students, faculty, departments, and courses efficiently without confusion or data loss.

