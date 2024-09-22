สวัสดีครับ
นี่คือการส่งแบบฝึกหัดแบบ febonacci การรับค่า 1-100 และคำนวณผลรวม โดยใช้ภาษา Javascript โดยใช้Node.js with Expressครับ 
ขั้นตอนการทำงานและข้อผิดพลาดที่พบ
1. ทำการnpm install express โดยจะได้ตัวไฟล์jsonมา แล้วตรวจว่ามี expressในjsonหรือไม่ รวมถึงการเข้าโมดูลด้วย
2. สร้างไฟล์ Javascript (ของผมชื่อ index.js)มี 1 ไฟล์ ในการทำโจทย์เป็นหลักครับ
3. ผมใช้port 3000 ,สร้างฟังก์ชันfibonacci โดยจำนวนที่รับค่าต้องไม่เกิน100,โดย_n คือจำนวนรับค่าที่ต้องไม่เกิน100,tempคือค่าfibonacciที่ถูกกำหนดไว้ในทฤษฎี
   โดยมีฟังก์ชันที่เมื่อจำนวนรับค่าเกิน100 เช่น101 จะติดerrorทันที แต่ถ้าเลข อยู่1-100 จะแสดงข้อมูลออกมา
4.ต่อมาเป็นฟังก์ชันผลรวมของค่าfibanacci โดยจะมีการรับพารามิเตอร์ และใช้ฟังก์ชันคำนวณลำดับ
5.ต่อมา ตรวจสอบว่าเกิดErrorหรือไม่ โดยผมกำหนดให้ 200 ตือ รันได้ผลลัพธ์ปกติ 400 คือ error 500 คือ เกิดข้อผิดพลาดในการคำนวณ Fibonacci
6.ขั้นตอนต่อมา ส่งค่าพอร์ต เพื่อทำการรัน
ในการทดสอบ เราจะใช้ Postman ทดสอบ โดยใช่GET เพื่อดูค่า และใช้URL http://localhost:3000/fibonacci/8  ตัวเลข 8 คือ จำนวนเลขที่เราต้องใส่ โดยมีเงื่อนไข ห้ามเกิน100
หรือ ติดลบ เป็น0 แม้กระทั่งไม่ใช่คค่า จะติด Error ทันที
ถ้าเกิดรันได้ปกติ จะเรียงค่าตั้งแต่น้อยไปมาก และผลรวมทั้งหมดในบรรทัดสุดท้าย
ข้อผิดภาพที่พบ
1.การวางตำแหน่งวงเล็บที่ไม่ดีของผมทำให้เกิดerrorในช่วงต้น
2.ความผิดพลาดในการนิยามตัวแปร
3.ในการแสดงผลยังมีerrorที่อาจมองไม่เข้าใจ เช่น ใส่ค่า101 ก็ยังขึ้น200 แต่ ไม่มีค่าลำดับปรากฏ ส่วน 0 ค่าติดลบ และไม่ใส่ค่า ติดerrorครับ
มีเรื่องปรับปรุงแก้ไขเพิ่มเติม สามารถแจ้งผมได้ครับ
ขอบคุณครับพี่ตะวัน



