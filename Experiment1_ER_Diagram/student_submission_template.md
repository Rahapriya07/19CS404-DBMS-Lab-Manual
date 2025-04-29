# ER Diagram Submission - Raha Priya Dharshini M

## Scenario Chosen:
University 

## ER Diagram:
![dbms exp-1](https://github.com/user-attachments/assets/36b29ae3-6c13-4821-92ec-0575a8c59ebd)


## Entities and Attributes:
Student: Name, DOB, Register Number, Phone Number, Email ID, Subjects Enrolled
University:University Name, University ID, Students and Faculties

Department:Department Name, Department ID

Program:Program Name, Program Code, Subjects

Faculties:Name, Subject, Faculty ID

Course:Course Name, Course Code, Credits

## Relationships and Constraints:
Relationship1 – Relationship (Many-to-Many, Student–University)

Relationship2 – Is in a (Many-to-Many, Student–Department)

Relationship3 – Provides (Many-to-Many, Department–Program)

Relationship4 – Contains (Many-to-Many, Program–Course)

Relationship5 – Handles (Many-to-Many, Faculties–Course)

Relationship6 – Has (Many-to-Many, University–Faculties)

## Extension (Prerequisite / Billing):
Explain how you modeled prerequisites or billing.
First, a self-referencing M:N
relationship called "Prerequisite" would be added within the Course entity, allowing
the system to model the dependency between different courses. This ensures that
course enrollment rules based on previous completions can be enforced properly.
Second, a new entity called "Payment" would be introduced and linked to the
Student entity through a One-to-Many relationship. This addition would help track
all financial transactions, manage tuition fees, and support billing operations,
providing a complete view of the financial obligations of each student. These
enhancements would make the model more realistic and capable of supporting a
fully functional university management system.

## Design Choices:
Brief explanation of why you chose certain entities, relationships, and assumptions.

 I choose entities, relationships, and assumptions based on their relevance to the core
functionality and objectives of the system being modeled. Entities represent the key
objects or components, such as "Customer" or "Order," that drive the system's
processes. Relationships define how these entities interact or depend on each other,
ensuring the workflow is captured accurately. Assumptions are made to simplify
complex scenarios and focus on what's essential, excluding unnecessary complexity.
These choices help in creating a practical, efficient, and scalable system that meets the
user's needs while reducing ambiguity.

