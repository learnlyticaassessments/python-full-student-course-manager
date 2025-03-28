# 🧠 Student Course Registration System

📁 **Filename:** `solution.py`  
🧪 **Difficulty:** Medium | **Total Marks:** 10  
📘 **Concepts:** OOP, Custom Exceptions, Dictionaries

---

## 📌 Problem Statement

Design a class-based system to manage course registrations for students. Each student can:

- Register for courses (no duplicates)
- Drop courses they are enrolled in
- View their current course list
- Count how many courses they are registered in

You must also implement proper exception handling for invalid operations.

---

## 🧱 Class + Exceptions to Implement

### Class: `StudentCourseManager`



### Custom Exceptions

```python

class StudentCourseManager:

function Description: 

register_course(self, student: str, course: str) -> str

function Description: 

drop_course(self, student: str, course: str) -> str:
        # Raises CourseNotFoundException if course doesn't exist

function Description: 
view_courses(self, student: str) -> list:
        # Returns a list of enrolled courses

function Description: 

get_total_courses(self, student: str) -> int:
        # Returns number of enrolled courses

Class Description:

class AlreadyRegisteredException(Exception):

Class Description:

class CourseNotFoundException(Exception):


---

## 🧪 Test Case Structure

| Test Case | Description | Marks |
|----------|-------------|-------|
| TC1 | Register a course | 2 |
| TC2 | Drop a course | 2 |
| TC3 | View registered courses | 2 |
| HTC1 | Duplicate registration | 2 |
| HTC2 | Dropping non-existent course | 2 |
