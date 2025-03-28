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

```python
class StudentCourseManager:
    def __init__(self):
        self.registrations = {}

    def register_course(self, student: str, course: str) -> str:
        # Raises AlreadyRegisteredException if already registered

    def drop_course(self, student: str, course: str) -> str:
        # Raises CourseNotFoundException if course doesn't exist

    def view_courses(self, student: str) -> list:
        # Returns a list of enrolled courses

    def get_total_courses(self, student: str) -> int:
        # Returns number of enrolled courses
```

### Custom Exceptions

```python
class AlreadyRegisteredException(Exception):
    pass

class CourseNotFoundException(Exception):
    pass
```

---

## 🧪 Test Case Structure

| Test Case | Description | Marks |
|----------|-------------|-------|
| TC1 | Register a course | 2 |
| TC2 | Drop a course | 2 |
| TC3 | View registered courses | 2 |
| HTC1 | Duplicate registration | 2 |
| HTC2 | Dropping non-existent course | 2 |

✅ **Visible test cases** show expected and actual  
🔒 **Hidden test cases** report pass/fail only

---

## 🚀 How to Run Tests

### Step 1: Write your code in `solution.py`

Do not rename files.

---

### Step 2: Run the test script

```bash
python run.py
```

Or press ▶️ inside `run.py` in VS Code.

---

### Step 3: See your results

✅ Test outcomes will be shown in terminal  
📄 Results will be appended to `report.txt`

---

## 📄 Example Output (in `report.txt`)

```
Run on 2025-03-28 14:42:01
✅ TC1: Register John for Math => ✅ Passed | Expected: John registered for Math, Got: John registered for Math
✅ TC2: Drop John from Math => ✅ Passed | Expected: John dropped Math, Got: John dropped Math
✅ TC3: View John's courses => ✅ Passed | Expected: [], Got: []
🔒 HTC1: Register John for Math again (Duplicate) => ✅ Passed (Exception caught)
🔒 HTC2: Drop unregistered course => ✅ Passed (Exception caught)
```

---

## 📤 Submitting Your Work

Once you're ready:
- Save all changes
- Run tests to ensure `report.txt` is up to date
- Use the Learnlytica extension to **Submit Assignment**

---

🎉 Good luck from Team Learnlytica!