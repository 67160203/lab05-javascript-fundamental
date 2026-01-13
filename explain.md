# Explain Code 5: JavaScript Fundamentals

## 01-variables.js - 6. Challenge: Create a Person Object

### Result

=== Challenge: Person Object ===<br>
Student object:<br>
{<br>
firstName: 'Alice',<br>
lastName: 'Smith',<br>
age: 20,<br>
gpa: 3.8,<br>
courses: [ 'HTML', 'CSS', 'JavaScript' ],<br>
isActive: true,<br>
getFullName: [Function: getFullName],<br>
getInfo: [Function: getInfo]<br>
}<br>
Full name: Alice Smith<br>
Info: Alice Smith, Age: 20, GPA: 3.8<br>
Courses: HTML, CSS, JavaScript<br>

### Explain

โค้ดนี้จะเป็นการแสดงชื่อจริง ข้อมูล อายุ เกรด และภาษาโค้ดที่ผู้ใช้ศึกษา ฟังก์ชัน getFullName จะเป็นฟังก์ชันที่นำชื่อจริง และนามสกุลของผู้ใช้มารวมกันไว้ที่เดียว เพื่อที่เวลาเรียกใช้จะสามารถเรียกได้พร้อมกันโดยที่ไม่ต้องเรียกทีละตัว ส่วนฟังก์ชัน getInfo จะเป็นฟังก์ชังที่นำ ชื่อเต็ม ข้อมูล อายุ และเกรด มารวมเข้าด้วยกัน
