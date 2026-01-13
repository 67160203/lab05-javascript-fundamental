# Explain Code 5: JavaScript Fundamentals

## 01-variables.js - 6. Challenge: Create a Person Object

### Result 6. Challenge: Create a Person Object

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

โค้ดนี้จะเป็นการแสดงชื่อจริง ข้อมูล อายุ เกรด และภาษาโค้ดที่ผู้ใช้ศึกษา ฟังก์ชัน getFullName จะเป็นฟังก์ชันที่นำชื่อจริง และนามสกุลของผู้ใช้มารวมกันไว้ที่เดียว เพื่อที่เวลาเรียกใช้จะสามารถเรียกได้พร้อมกันโดยที่ไม่ต้องเรียกทีละตัว ส่วนฟังก์ชัน getInfo จะเป็นฟังก์ชันที่นำ ชื่อเต็ม ข้อมูล อายุ และเกรด มารวมเข้าด้วยกัน เพื่อให้แสดงออกมาพร้อมกัน

---

## 02-functions.js - 8. Returning Objects, 9. Function as Parameter (Callback)

### Result 8. Returning Objects

Returning Objects:<br>
{<br>
firstName: 'John',<br>
lastName: 'Doe',<br>
age: 30,<br>
email: 'john.doe@example.com',<br>
getFullName: [Function: getFullName],<br>
getAge: [Function: getAge]<br>
}<br>
Email: john.doe@example.com<br>
Full name: John Doe<br>

### Explain

โค้ดนี้จะเป็นการสร้างฟังก์ชันขึ้นมาเพื่อส่งค่าที่รับมาจากผู้ใช้กลับออกไป และมีการแปลงค่าบางตัวให้กลายเป็นค่าใหม่อีกด้วย โดยส่วนขอฟังก์ชัน getFullName และ getAge จะเป็นการคืนค่าไปโดยตรง แต่ในส่วนของ email จะมีการแปลงค่าจากผู้ใช้ โดยนำชื่อจริงและนามสกุลมาทำให้เป็นตัวพิมพ์เล็กให้หมด พร้อมทั้งมี . คั่นระหว่างสองค่า และใส่ @example.com ตามหลัง เพื่อให้ทราบว่าค่านี้เป็นอีเมลที่ถูกแปลงมาจากชื่อจริง และนามสกุลของผู้ใช้

### Result 9. Function as Parameter (Callback)

Callback Function:<br>
Original: [ 1, 2, 3, 4, 5 ]<br>
Doubled: [ 2, 4, 6, 8, 10 ]<br>
Squared: [ 1, 4, 9, 16, 25 ]<br>

### Explain

โค้ดนี้จะเป็นโค้ดเกี่ยวกับการคืนของ array ออกมา โดยจะให้ callback เป็นตัวคำนวณค่าต่างๆที่ถูกส่งเข้าไปตามสมการที่ได้เขียนไว้ เมื่อคำนวณเสร็จค่าที่เปลี่ยนไปจะถูกส่งออกมาเป็นค่าดับเบิ้ลและค่าที่ถูกยกกำลัง

---

## 03-control-flow.js - 5. Short-Circuit Evaluation, 7. Form Validation

### Result 5. Short-Circuit Evaluation

Short-Circuit Evaluation:<br>
User name: John<br>
User profile: undefined<br>

### Explain

โค้ดนี้จะเป็นการแสดงการตรวจสอบข้อมูลโดยมีการใช้ || ซึ่งตัวนี้จะเป็นการตรวจสอบข้อมูลจากซ้ายไปขวา ถ้าตัวแรกใช้ไม่ได้ก็จะไปตรวจสอบที่ตัวต่อไป ส่วน && จะตรวจสอบก่อนใช้งาน ซึ่งหมายความว่าจะต้องมีตัวแรกก่อนถึงจะไปตรวจสอบตัวถัดไปได้ และสุดท้าย ?. เป็นการเช็คว่ามีตัวหน้าหรือไม่ ถ้าไม่มีก็ไม่ต้องเอาค่าของตัวถัดไปมา แต่ถ้ามีก็ให้นำค่าตัวถัดไปมาด้วย

### Result 7. Form Validation

Form Validation:<br>
Valid user: { isValid: true, errors: [] }<br>
Invalid user: {<br>
isValid: false,<br>
errors: [<br>
'Name must be at least 3 characters',<br>
'Valid email is required',<br>
'Must be 18 or older',<br>
'Password must be at least 6 characters',<br>
'Must agree to terms'<br>
]<br>
}<br>

### Explain

โค้ดนี้คือตัวตรวจสอบฟอร์มสมัครสมาชิก ตรวจสอบว่า ผู้ใช้กรอกข้อมูลมาถูกต้อง และผ่านเงื่อนไขหรือไม่ ถ้ามีอะไรไม่ครบหรือไม่ผ่านเงื่อนไขก็จะขึ้นว่าไม่ผ่าน และนำค่าที่ไม่ถูกต้องไปแสดงตรง error ส่วนถ้าข้อมูลถูกต้องหมดก็จะไม่มีการแสดงอะไร

---

## 04-loops.js - 9. Chaining methods, 10. Challenge: Student Grades

### Result 9. Chaining methods

Method chaining:<br>
Even numbers squared: 2²=4, 4²=16, 6²=36, 8²=64, 10²=100<br>
Average: 30<br>

### Explain

โค้ดนี้จะอธิบายเกี่ยวกับ method chaining ซึ่งนั่นก็คือการนำเอา array มาทำหลายอย่างในทีเดียวกัน โดยที่เราจะใส่สมการไว้ใน const evenStrings และให้มันคำนวณค่าจาก data ที่เราพิมไว้ และในส่วนของ const average จะเป็นการหาค่าเฉลี่ยจาก numbers2 และสุดท้ายก็ส่งค่าออกมาแสดงผล

### Result 10. Challenge: Student Grades

Challenge: Student Analysis<br>
Students: [<br>
{ name: 'Alice', score: 95 },<br>
{ name: 'Bob', score: 75 },<br>
{ name: 'Charlie', score: 85 },<br>
{ name: 'Diana', score: 92 },<br>
{ name: 'Eve', score: 88 }<br>
]<br>
Names: Alice, Bob, Charlie, Diana, Eve<br>
High scorers: Alice (95), Charlie (85), Diana (92), Eve (88)<br>
Class average: 87.00<br>
Top scorer: Alice (95)<br>
Summary (sorted):<br>
Alice: 95 (A)<br>
Diana: 92 (A)<br>
Eve: 88 (B)<br>
Charlie: 85 (B)<br>
Bob: 75 (C)<br>

### Explain

โค้ดนี้จะเกี่ยวกับการแสดงชื่อ คะแนน และผลการเรียนของนักเรียนแต่ละคน โดย const students จะเป็นตัวที่เก็บทั้งชื่อนักเรียน และคะแนนสอบไว้ในที่เดียวกัน ส่วน const names จะเป็นการดึงแค่ชื่อของนักเรียนออกมาจาก const students ต่อมา const highScorers จะเอาไว้เก็บแค่เฉพาะนักเรียนที่มีคะแนนมากกว่า 85 เพื่อไปแสดง const classAverage เป็นการนำคะแนนของทุกคนในห้องมาค่าเฉลี่ยนเพื่อนำไปแสดงผล const topScorer จะใช้หาว่าใครได้คะแนนเยอะที่สุดในห้อง โดยจะใช้การเปรียบเทียบคะแนนของแต่ละคนไปเรื่อยๆ จนได้คนที่คะแนนมากที่สุด และสุดท้าย const summary จะเป็นการสรุปข้อมูลของนักเรียนทั้งหมด และมีการคำนวณเกรดออกมาจากคะแนนเอาไว้ให้อีกด้วย

---

## 05-integration.js - Activity 5: Integration - Quiz Application

### Result Activity 5: Integration - Quiz Application

🎯🎯 === QUIZ APPLICATION === 🎯🎯

QUIZ RESULTS:
────────────────────────────────────────────────────────────
Q1: What is 5 + 3?
Your answer: 6
Correct answer: 8
❌ WRONG

Q2: What is the capital of Thailand?
Your answer: Bangkok
✅ CORRECT

Q3: What is the largest planet?
Your answer: Saturn
Correct answer: Jupiter
❌ WRONG

Q4: What is 2^8?
Your answer: 512
Correct answer: 256
❌ WRONG

Q5: Which is NOT a JavaScript data type?
Your answer: boolean
Correct answer: class
❌ WRONG

────────────────────────────────────────────────────────────
FINAL SCORE: 1/5 (20.0%)
GRADE: F

FEEDBACK:
💪💪 Keep practicing. You'll improve!

📊📊 STATISTICS:
Total questions: 5
Correct: 1
Incorrect: 4
Success rate: 20.0%

Answer breakdown:
✅ Correct: 1
❌ Incorrect: 4

✅ All activities completed!

### Explain

โค้ดนี้เป็นโค้ดเกี่ยวกับโปรแกรมทำข้อสอบ ตัวแรก const quizzes จะเป็นการใส่คำถามที่เราต้องการจะถามลงไป จำนวนกี่ข้อก็ได้ ซึ่งในนั้นจะต้องมีช้อยส์ให้เลือก และกำหนดข้อที่ถูกไว้ด้วย ต่อมา quizzes.forEach เป็นการหยิบคำถามแต่ละข้อขึ้นมา และทำให้ครบทุกข้อ ในส่วน const userAnswer จะเป็นการใช้ Math.floor(Math.random() \* 4); สมการเพื่อจำลองการทำข้อสอบ และคำตอบจะถูกสุ่มทุกครั้ง และนำไปคูณ 4 เพราะเรามีช้อยส์ทั้งหมด 4 ตัว ถ้าตอบถูกจะถูกเก็บไว้ที่ const isCorrect แล้ว results.push จะเป็นการเก็บข้อมูลว่าเรากำลังทำข้อสอบข้อไหน คำถามคืออะไร คำตอบคืออะไร คำตอบที่ถูกคืออะไร และเราทำถูกหรือไม่ results.forEach(result) จะเป็นการแสดงคำตอบที่ถูกต้องของแต่ละข้อ และในส่วนนี้ const correctCount จะเป็นการคำนวณคะแนนรวมทั้งหมดที่ทำได้ ซึ่งคะแนนตรงนี้จะถูกส่งต่อไปคำนวณเพื่อเป็นคะแนน และคำนวณเป็นเกรดเพื่อแสดงออกมาให้ผู้ใช้ได้รู้ และสุดท้าย const byCorrectness จะเป็นการบอกว่าผู้ใช้ตอบผิด และตอบถูกไปกี่ข้อ
