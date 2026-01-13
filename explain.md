# Explain Code 5: JavaScript Fundamentals

## 01-variables.js - 6. Challenge: Create a Person Object

### Result

=== Challenge: Person Object ===
Student object:
{
firstName: 'Alice',
lastName: 'Smith',
age: 20,
gpa: 3.8,
courses: [ 'HTML', 'CSS', 'JavaScript' ],
isActive: true,
getFullName: [Function: getFullName],
getInfo: [Function: getInfo]
}
Full name: Alice Smith
Info: Alice Smith, Age: 20, GPA: 3.8
Courses: HTML, CSS, JavaScript

### Explain

โค้ดนี้จะเป็นการแสดงชื่อจริง ข้อมูล อายุ เกรด และภาษาโค้ดที่ผู้ใช้ศึกษา ฟังก์ชัน getFullName จะเป็นฟังก์ชันที่นำชื่อจริง และนามสกุลของผู้ใช้มารวมกันไว้ที่เดียว เพื่อที่เวลาเรียกใช้จะสามารถเรียกได้พร้อมกันโดยที่ไม่ต้องเรียกทีละตัว ส่วนฟังก์ชัน getInfo จะเป็นฟังก์ชังที่นำ ชื่อเต็ม ข้อมูล อายุ และเกรด มารวมเข้าด้วยกัน
