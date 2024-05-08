# EX-01 ER Diagram

### AIM:
To analyze the problem and come with the entities in it and identify the constraints in creating the database.
### Scenario 1: University Database
Consider a university database system designed to manage information about students, courses,
instructors, and the enrollment of students in courses. The university offers various programs, and
each program consists of multiple courses.

### User Requirements:
The university offers various academic programs that are grouped under different departments.
Details that need to be captured for each program include a unique identifier, program name and
the governing department.

The university has a list of students enrolled across different programs offered. For every student,
details like unique admission number, full name, date of birth, contact information such as email
and phone number need to be stored.

There are multiple instructors in the university teaching one or more courses. Relevant details for
each instructor required include unique staff number, name, contact information like phone and
email.

The university offers a catalog of courses across programs. Each course taught requires capturing
course number, name, number of credits/units etc
Students can enroll or register in one or more courses in a given academic term. The system needs
to track details like which student has enrolled in which particular course(s) and date of enrollment
for reporting requirements.

### Tasks.
Create an ER diagram for the University Database based on the given scenario

### ER Diagram
![Screenshot 2024-05-08 142405](https://github.com/syedmokthiyar/DBMS--EX-01/assets/118787294/01cc6b2c-eef7-44d6-a6dd-b5dee4c0cd02)


### Explanation
Entities

Student: Represents an individual enrolled in a university program. Course: Represents a specific
academic course offered by the university. Program: Represents a degree program or major offered
by the university University: Represents the institution itself. Department: Represents a specific
department within the university. Mentor. Represents a faculty member or advisor assigned to a
student. 

Relationships

A Student is enrolled in a Program. A Program is offered by a University. A Course is part of a
Program. A Course has Prerequisites, which are other courses that must be completed before
taking the course. A Student has Attempts at a Course, which represents their enrollment and grade
history. A Department offlers Courses

Prerequisites:

The concept of prerequisites is implemented through the Contains relationship between Courses.
This allows for the representation of hierarchical dependencies between courses, where a course
may have one or more prerequisites that must be completed before it can be taken. For example, a
course in calculus may have a prerequisite of algebra, indicating that students must complete
algebra before enrolling in calculus
The Prerequisites relationship is likely implemented as a many-to-many relationship, allowing a
coume to have multiple prerequisites and a prerequisite course to be required for multiple courses.

Overall, this entity-relationship model appears to be designed to manage student, enrollment,
course offerings, and program requirements, while also ensuring that students meet the necessary
prerequisites for each course

### Scenario 2: Hospital Database

The Hospital Management System is a tailored operational model for healthcare institutions. Its
primary function is to efficiently register, store, and retrieve patient and doctor details, allowing
meaningful manipulation of the data.

### User Requirements:
#### Patient Management
The hospital needs to manage information about patents, mehuring the birth, gender, address,
contact information phone number, email, and Doctor Manage

The hospital employs multiple doctors, sach identified by a unique Doctor Doctor specialization,
contact information phone number, emarts, and work schedule Department Management

The hospital consists of various departments teg, cardiology, pediatres, oncology Sach depart
identified by a unique DepartmentID Appointment Scheduling and has attributes such as
Departmenthame andPatients can schedule appointments with doctors for medical consultations or procedures.

Each app has a unique AppointmentID and is associated with a specific patient and doctor. Apporters d
appointment date and time, reason for the visit, and any additional notes Medical Racords
The hospital needs to maintain electronic medical records for each patient visit.

Medical reconds include information about diagnoses, prescribed medications, treatments, test results, and any
other relevant medica information. Each medical record is associated with a specific patient and
doctor and has a unique MedicalRecordID.

### Tasks
Create an ER diagram for the Hospital Database based on the given scenario Identify entities, relationships, and attributes. Specify cardinality and participation constraints.

### ER Diagram
![Screenshot 2024-05-08 143423](https://github.com/syedmokthiyar/DBMS--EX-01/assets/118787294/97e83bf7-7a90-4ec4-b54f-914a50035086)


### Explanation
The entities include:
Patient Information
Doctors (identified by Doctorate)
Adristos dertified by Asia
Services (identified by Service Name)
Rooms (identified by Room)
Departments Identified by Departments, such as Pediatrics, Candogand
Bills (identified by InPatient Bill and Outpatient B
Appointments (identified by Appointmenti
Hospital (a single entity)
Outpatient Medical Info identified by Outpatient MediD)
The relationships between these entities seem to capture the following

A patient can have multiple admissions, and each admission is associated with a service, room, and
department.A doctor can attend to multiple patients, and each patient is assigned to a doctor A
patient can have multiple bills, and each bill is associated with a payment collected by a casfuer
Regarding billing and payment, Inpatient bills are associated with admissions, while outpatient bils
are associated with appointments. The "Collected by" attribute suggests that the model tracks who
collects the payment for each bill.


### Result:
Thus, To analyze the problem and come with the entities in it and identify the constraints in creating the database is done successfully.


