
# Day 6 – Triggers & SOQL

---

# 1. What is SOQL?

SOQL (Salesforce Object Query Language) is a query language used in Salesforce to retrieve data from objects.

It is similar to SQL but designed specifically for Salesforce objects and relationships.

### Example:
```sql
SELECT Name, Email FROM Contact
```

SOQL is used to:
- Retrieve records from Salesforce objects
- Filter records using conditions
- Access related objects
- Perform aggregate operations

---

# 2. What is an Apex Trigger?

An Apex Trigger is a piece of Apex code that executes automatically when records are inserted, updated, deleted, or undeleted in Salesforce.

Triggers help automate business processes and enforce business rules.

### Example Use Cases:
- Send notifications
- Update related records
- Validate data
- Create tasks automatically

### Example Trigger:
```apex
trigger AccountTrigger on Account(before insert) {

    for(Account acc : Trigger.new) {
        acc.Description = 'New Account Created';
    }
}
```

---

# 3. Differences

## Flow vs Trigger

| Flow | Apex Trigger |
|------|---------------|
| No-code/low-code automation | Code-based automation |
| Easy to build and maintain | Used for complex logic |
| Best for simple business processes | Best for advanced processing |
| Drag-and-drop interface | Requires Apex programming |
| Limited for complex integrations | Supports complex integrations and APIs |

---

## Before Trigger vs After Trigger

| Before Trigger | After Trigger |
|----------------|----------------|
| Executes before saving records | Executes after saving records |
| Used to update/validate fields | Used for related records and actions |
| Faster because no extra save needed | Used when record ID is required |
| Example: Set default values | Example: Create related tasks |

---

# 4. Trigger Use Cases

## Case 1: Student Registration
- Trigger Event: After student record creation
- Action: Send welcome email to student.

## Case 2: Low Attendance
- Trigger Event: After attendance update
- Action: Send warning notification if attendance drops below 75%.

## Case 3: Course Full
- Trigger Event: After enrollment count reaches limit
- Action: Notify faculty that the course is full.

## Case 4: Fee Payment Completed
- Trigger Event: After fee status changes to Paid
- Action: Generate fee receipt automatically.

## Case 5: Faculty Assignment
- Trigger Event: After faculty assigned to course
- Action: Notify faculty and update schedule.

---

# 5. Query Examples

### Query 1
Find all students enrolled in Course A.

### Query 2
Find all courses handled by Faculty X.

### Query 3
Find students with attendance below 75%.

### Query 4
Find students with pending fee payments.

### Query 5
Find all courses that are fully occupied.

### Query 6
Find faculty assigned to more than three courses.

---

# 6. Reflection

## Why enterprise systems react automatically to data changes

Enterprise systems manage large amounts of business data and operations continuously. Automatic reactions to data changes help organizations improve efficiency and reduce manual work.

### Reasons:
- Automates repetitive tasks
- Provides real-time notifications
- Improves accuracy and consistency
- Reduces human errors
- Supports faster business decisions
- Enhances user experience
- Helps systems communicate with each other

In a College Management System, automatic reactions help manage attendance, fee processing, student communication, faculty notifications, and course management efficiently.




# Core Task

# College Management System – Event Driven Design Tasks

## 1. Trigger Thinking

### Case 1: Student Registration
- **Trigger Event:** After a new student record is created
- **Automatic Action:** Send a welcome email with login credentials and course details.

### Case 2: Course Capacity Reached
- **Trigger Event:** After course enrollment count reaches maximum capacity
- **Automatic Action:** Notify faculty and administration that the course is full.

### Case 3: Low Attendance Warning
- **Trigger Event:** After attendance percentage falls below 75%
- **Automatic Action:** Send a warning notification to the student and parents.

### Case 4: Fee Payment Completion
- **Trigger Event:** After student fee status changes to "Paid"
- **Automatic Action:** Generate fee receipt and update student financial records.

### Case 5: Faculty Assignment Update
- **Trigger Event:** After a faculty member is assigned to a course
- **Automatic Action:** Notify the faculty member and update the course schedule.

---

# 2. Flow vs Trigger Thinking

| Scenario | Solution | Reason |
|----------|----------|---------|
| Simple email notification | Flow | Easy to configure and maintain without coding. |
| Complex fee eligibility check | Apex Trigger | Requires complex business logic and validations. |
| Updating related records | Flow | Suitable for simple automation between related records. |
| External API integration | Apex Trigger | Requires callouts and advanced integration logic. |
| Attendance warning automation | Flow | Can be implemented using conditions and notifications. |

---

# 3. Query Thinking

### Query 1
Find all students enrolled in Course A.

### Query 2
Find all courses handled by Faculty X.

### Query 3
Find students whose attendance is below 75%.

### Query 4
Find students who have pending fee payments.

### Query 5
Find courses that have reached maximum capacity.

### Query 6
Find faculty members assigned to more than three courses.

---

# 4. Reflection Task

## Why do enterprise systems need event-driven behavior?

Enterprise systems manage large volumes of data and multiple business operations simultaneously. Event-driven behavior allows the system to respond automatically whenever important changes occur.

### Benefits:
- Automates repetitive business processes
- Provides real-time notifications and updates
- Maintains data accuracy and consistency
- Improves scalability and performance
- Enhances user experience
- Enables integration between multiple systems

In a College Management System, event-driven behavior helps automate student registration, attendance tracking, fee processing, faculty notifications, and course management efficiently.
