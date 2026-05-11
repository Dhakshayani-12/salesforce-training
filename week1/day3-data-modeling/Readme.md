# Day 3 – Data Modeling (College Management System)

# CORE TASKS

---

# 1️⃣ Design a College Management System

## Objects

### Student
Stores student-related information.

Fields:
- Student ID
- First Name
- Last Name
- Email
- Age
- Department
- Course

---

### Faculty
Stores faculty/teacher details.

Fields:
- Faculty ID
- Faculty Name
- Email
- Department

---

### Course
Stores course information.

Fields:
- Course Name
- Course Code
- Total Seats
- Enrolled Students
- Faculty
- Department

---

### Department
Stores department details.

Fields:
- Department Name
- HOD Name
- Total Students

---

# Relationships

## 1. Department → Student
- One department can have many students
- Relationship Type: One-to-Many
- Suggested Relationship: Lookup

Reason:
Each student belongs to one department, while a department contains multiple students.

---

## 2. Department → Faculty
- One department can have many faculty members
- Relationship Type: One-to-Many
- Suggested Relationship: Lookup

Reason:
Faculty members work under a single department.

---

## 3. Department → Course
- One department can offer many courses
- Relationship Type: One-to-Many
- Suggested Relationship: Lookup

Reason:
Courses are managed under departments.

---

## 4. Faculty → Course
- One faculty member can teach many courses
- Relationship Type: One-to-Many
- Suggested Relationship: Lookup

Reason:
A faculty member may handle multiple courses.

---

## 5. Course → Student
- One course can contain many students
- Relationship Type: One-to-Many
- Suggested Relationship: Lookup

Reason:
Many students can enroll in the same course.

---

# Data Model Diagram

```text id="2yngrf"
Department
   |
   |----< Student
   |
   |----< Faculty
   |
   |----< Course
                 |
                 |----< Students
                 |
                 |---- Faculty




## 1. Difference Between App, Object, Record, and Field

| Term | Meaning | Example |
|------|----------|----------|
| App | A collection of related features and objects used for a business purpose | College Management App |
| Object | A database table that stores similar types of data | Student Object |
| Record | A single entry inside an object | One student’s details |
| Field | A specific piece of information in a record | Student Name, Email |

---

# 2. Standard vs Custom Objects

## Standard Objects
These are objects already provided by platforms like Salesforce.

Examples:
- Account
- Contact
- Opportunity

## Custom Objects
These are user-created objects designed for specific business needs.

Examples in this project:
- Student
- Faculty
- Course
- Department

---

# 3. College Data Model

## Objects

### Student
Stores student information.

Fields:
- Student ID
- First Name
- Last Name
- Email
- Age
- Department
- Course

---

### Faculty
Stores faculty/teacher details.

Fields:
- Faculty ID
- Name
- Email
- Department

---

### Course
Stores course details.

Fields:
- Course Name
- Course Code
- Total Seats
- Enrolled Students
- Faculty
- Department

---

### Department
Stores department information.

Fields:
- Department Name
- HOD Name
- Total Students

---

# Relationships

## 1. Department → Student
One Department can have many Students.

Relationship Type:
- One-to-Many
- Lookup Relationship

Reason:
A student belongs to one department, but a department can contain many students.

---

## 2. Department → Faculty
One Department can have many Faculty members.

Relationship Type:
- One-to-Many
- Lookup Relationship

Reason:
Faculty members work under one department.

---

## 3. Department → Course
One Department can offer many Courses.

Relationship Type:
- One-to-Many
- Lookup Relationship

Reason:
Each course belongs to a department.

---

## 4. Faculty → Course
One Faculty member can teach many Courses.

Relationship Type:
- One-to-Many
- Lookup Relationship

Reason:
A faculty member may handle multiple courses.

---

## 5. Course → Student
One Course can contain many Students.

Relationship Type:
- One-to-Many
- Lookup Relationship

Reason:
Many students enroll in a course.

---

# Data Model Diagram

```text
Department
   |
   |----< Student
   |
   |----< Faculty
   |
   |----< Course
                 |
                 |----< Students
                 |
                 |---- Faculty
