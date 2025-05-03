# Experiment 1: Entity-Relationship (ER) Diagram

## 🎯 Objective:
To understand and apply the concepts of ER modeling by creating an ER diagram for a real-world application.

## 📚 Purpose:
The purpose of this workshop is to gain hands-on experience in designing ER diagrams that visually represent the structure of a database including entities, relationships, attributes, and constraints.

---

### 🔹 Scenario: University Database
Design a database to manage students, instructors, programs, courses, and student enrollments. Include prerequisites for courses.

**User Requirements:**
- Academic programs grouped under departments.
- Students have admission number, name, DOB, contact info.
- Instructors with staff number, contact info, etc.
- Courses have number, name, credits.
- Track course enrollments by students and enrollment date.
- Add support for prerequisites (some courses require others).


---

## 📝 Tasks:
1. Identify entities, relationships, and attributes.
2. Draw the ER diagram using any tool (draw.io, dbdiagram.io, hand-drawn and scanned).
3. Include:
   - Cardinality & participation constraints
   - Prerequisites for University OR Billing for Hospital
4. Explain:
   - Why you chose the entities and relationships.
   - How you modeled prerequisites or billing.

# ER Diagram Submission - Student Name
![212223100044](https://github.com/user-attachments/assets/08200937-10f6-4fd8-bb8c-4e4701ca272f)

## Scenario Chosen:
University 


## Entities and Attributes:
- Entity1: Student
- Entity2: Course
- Entity3: Instructor
- Entity4: Department
- Entity5: Classroom
...

## Relationships and Constraints:
- Enrollment (Student–Course) → (1:N, total-total)
- Teacher (Course–Instructor) → (N:1, total-partial)
- Belongs (Course–Department) → (N:1, total-partial)
- Schedule (Course–Classroom–Instructor) → (1:N, total-total)
...

## Extension (Prerequisite / Billing):
For prerequisites, model it as a recursive relationship on the Course entity, where one course can have multiple prerequisite courses (many-to-many, partial participation).

For billing, add a Billing entity linked to Student in a one-to-many relationship, where each student can have multiple bills, and every bill belongs to one student (1:N, partial-total participation).

## Design Choices:
I chose entities like Student, Course, Instructor, Department, and Classroom to clearly represent core components of the system. Relationships like Enrollment, Schedule, and Teacher capture interactions between these entities. I assumed students can enroll in multiple courses, instructors can teach multiple courses, and classrooms can host different schedules, ensuring flexibility and real-world mapping.
## RESULT
Thus, an ER diagram for university database is created.
