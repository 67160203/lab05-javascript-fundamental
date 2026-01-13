# Explain Code 5: JavaScript Fundamentals

## 01-variables.js - 6. Challenge: Create a Person Object

### Result

=== Challenge: Person Object ===/n
Student object:/n
{/n
firstName: 'Alice',/n
lastName: 'Smith',/n
age: 20,/n
gpa: 3.8,/n
courses: [ 'HTML', 'CSS', 'JavaScript' ],/n
isActive: true,/n
getFullName: [Function: getFullName],/n
getInfo: [Function: getInfo]/n
}/n
Full name: Alice Smith/n
Info: Alice Smith, Age: 20, GPA: 3.8/n
Courses: HTML, CSS, JavaScript/n

### Explain

โค้ดนี้จะเป็นการแสดงชื่อจริง ข้อมูล อายุ เกรด และภาษาโค้ดที่ผู้ใช้ศึกษา ฟังก์ชัน getFullName จะเป็นฟังก์ชันที่นำชื่อจริง และนามสกุลของผู้ใช้มารวมกันไว้ที่เดียว เพื่อที่เวลาเรียกใช้จะสามารถเรียกได้พร้อมกันโดยที่ไม่ต้องเรียกทีละตัว ส่วนฟังก์ชัน getInfo จะเป็นฟังก์ชังที่นำ ชื่อเต็ม ข้อมูล อายุ และเกรด มารวมเข้าด้วยกัน
