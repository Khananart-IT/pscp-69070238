1.ข้อมูล OJ

หมายเลข/ชื่อโจทย์ OJ: oj3011 - Colors

OJ submission ID ถ้ามีการส่งแล้ว: 542423

สถานะ OJ: Passed

เวลาที่ใช้คิดและทำโจทย์ด้วยตนเอง: 30-60 minutes

2.ความเข้าใจโจทย์ของฉัน

อธิบายโจทย์: โจทย์ให้ทำโปรแกรมผสมสีระหว่างแม่สี 2 สี(น้ำเงิน,เหลือง,แดง) แล้วโปรแกรมจะให้ผลลัพธ์มาว่าจะได้สีอะไร

Input: 1.ชื่อสีที่ 1 2.ชื่อสีที่ 2

Output: สีที่ผสมออกมาได้ (หากข้อมูลที่กรอกไปไม่ใช่แม่สีให้ขึ้นผลลัพธ์ว่า "Error")

Constraints: ต้องทำเงื่อนไขหลายอย่าง เช่น กรณีที่แม่สีใน input ปกติ กรณีที่มีสีที่ไม่ใช่แม่สีมาใน input รวมถึงอาจมีกรณีที่มีแม่สีเดียวกันผสมกัน

3.แผนแรกของฉัน

ขั้นแรก: สร้าง input เพื่อรับค่าของชื่อสีที่ 1 และชื่อสีที่ 2

ขั้นที่สอง: สร้างข้อมูล list สำหรับข้อมูลของแม่สี

ขั้นที่สาม: สร้างเงื่อนไขหากสีใน input เป็นแม่สีต่างกันในข้อมูล list ก็จะส่งผลลัพธ์เป็นสีที่ต่างกันออกไป

ขั้นที่สี่: สร้างเงื่อนไขหากสีใน input ไม่เป็นแม่สีในข้อมูล list ก็จะส่ง output เป็น error

ขั้นที่ห้า: สร้างเงื่อนไขหากสีใน input เป็นแม่สีเดียวกันในข้อมูล list จะส่ง output เป็นสีเดิมของสีใน input

4.วิธีสุดท้ายที่ใช้จริง: วิธีสุดท้ายเหมือนกับวิธีแรกแต่อาจจะมีเงื่อนไขที่ค่อนข้างซับซ้อนเพื่อให้โปรแกรมสามารถรันได้ครอบคลุม input ที่ใส่เข้ามาได้มากยิ่งขึ้น

5.การทดสอบของฉัน

Case 1

ทำไมเลือก case นี้: เป็นแม่สีที่ต่างกันทั้งหมด

Input: 1.Yellow 2.Red

Expected output: Orange

Actual output: Orange

Result: Pass

Case 2

ทำไมเลือก case นี้: มี 1 สีที่ไม่ใช่แม่สี

Input: 1.Blue 2.White

Expected output: Error

Actual output: Error

Result: Pass

Case 3

ทำไมเลือก case นี้: เป็นแม่สีเดียวกันทั้ง 2 สี

Input: 1.Red 2.Red

Expected output: Red

Actual output: Red

Result: Pass

Case 4

ทำไมเลือก case นี้: ไม่เป็นแม่สีทั้ง 2 สี

Input: 1.White 2.Brown

Expected output: Error

Actual output: Error

Result: Pass

6.การใช้ AI
ใช้ AI กับโจทย์นี้หรือไม่: No

7.ความช่วยเหลือจากคน / การร่วมมือ
ได้ถามเพื่อน TA ผู้สอน หรือบุคคลอื่นเพื่อขอความช่วยเหลือในโจทย์นี้หรือไม่: No

ใครช่วยคุณ: ไม่มีใคร

ช่วยเหลือแบบใด: ไม่ได้ใช้ความช่วยเหลือจากคน

คุณยังทำอะไรด้วยตนเอง:
ฉันเขียนโปรแกรมเอง เลือก test cases เอง รันโปรแกรมใน VS Code เอง และส่งเข้า OJ ด้วยตนเอง

คุณคัดลอก code จากคนอื่นหรือไม่: No

8.คำรับรองของนักศึกษา

| Statement | Yes/No |
|---|---|
| I wrote this submission in my own words. | Yes |
| I understand my final code. | Yes |
| I recorded the real OJ status. | Yes |
| I did not copy AI-generated text directly into this file. | Yes |
| I did not copy code from another person. | Yes |
| If I received human help, I disclosed it in this file. | Yes |
| I submitted the final code to the OJ by myself. | Yes |
