## 1.ข้อมูล OJ

หมายเลข/ชื่อโจทย์ OJ: oj3536 - isPrime_large

OJ submission ID ถ้ามีการส่งแล้ว: 669136

สถานะ OJ: Passed

เวลาที่ใช้คิดและทำโจทย์ด้วยตนเอง: 30-60 minutes

## 2.ความเข้าใจโจทย์ของฉัน

อธิบายโจทย์: โจทย์นี้จะให้สร้างโปรแกรมว่าเลขที่รับค่าเข้ามาเป็นจำนวนเฉพาะหรือไม่

Input: 

    บรรทัดที่ 1 จำนวนนับใดๆ
 
Output: ถ้าเป็นจำนวนเฉพาะ "YES", ถ้าไม่ "NO"

Constraints: เลขที่รับค่าเข้ามาไม่ได้ระบุขอบเขตมาเพราะฉะนั้นเลขที่รับเข้ามาอาจจะเป็นเลขที่มีค่าสูงมากจนทำให้เกิด timeout ไเ้หากใช้วิธีการปกติ

## 3.แผนแรกของฉัน

ขั้นแรก: รับค่าเข้ามาถ้าค่าน้อยกว่าหรือเท่ากับ 1 ให้แสดงผล "NO" ทันที

ขั้นที่สอง: สร้าง limit เพื่อทำขอบเขตและลดเวลาการคำนวณ

ขั้นที่สาม: สร้าง for loop เพื่อคำนวณว่าเป็นจำนวนเฉพาะหรือไม่ โดยใช้ NUMBER % (i ** 2)

ขั้นที่สี่: แสดงผลว่าเป็นจำนวนเฉพาะหรือไม่


## 4.วิธีสุดท้ายที่ใช้จริง:
วิธีสุดท้ายของฉันมีพื้นฐานจากวิธีแรกแต่มีการปรับเปลี่ยนในตัว for loop ให้เป็น NUMBER % i แทนและเปลี่ยน ตัวขอบเขตใน for loop จาก 1, limit เป็น 2, limit + 1 แทน

### Case 1

ทำไมเลือก case นี้: ถ้าตัวเลขเป็นจำนวนมากๆจะเป็นอย่างไร

Input: 14785239425636945236715283

Expected output: NO

Actual output: NO

Result: Pass

### Case 2

ทำไมเลือก case นี้: ถ้าเป็นจำนวนติดลบจะเป็นอย่างไร

Input: -1236545454121265

Expected output: NO

Actual output: NO

Result: Pass

### Case 3

ทำไมเลือก case นี้: ถ้าเป็นจำนวนเฉพาะที่มีค่ามากๆจะเป็นอย่างไร

Input: 1000000181

Expected output: YES

Actual output: YES

Result: Pass

## 6.การใช้ AI
ใช้ AI กับโจทย์นี้หรือไม่: Yes
## 7.ความช่วยเหลือจากคน / การร่วมมือ
ได้ถามเพื่อน TA ผู้สอน หรือบุคคลอื่นเพื่อขอความช่วยเหลือในโจทย์นี้หรือไม่: No

ใครช่วยคุณ: ไม่มีใคร

ช่วยเหลือแบบใด: ไม่ได้ใช้ความช่วยเหลือจากคน

คุณยังทำอะไรด้วยตนเอง:
ฉันเขียนโปรแกรมเอง เลือก test cases เอง รันโปรแกรมใน VS Code เอง และส่งเข้า OJ ด้วยตนเอง

คุณคัดลอก code จากคนอื่นหรือไม่: No

## 8.คำรับรองของนักศึกษา

| Statement | Yes/No |
|---|---|
| I wrote this submission in my own words. | Yes |
| I understand my final code. | Yes |
| I recorded the real OJ status. | Yes |
| I did not copy AI-generated text directly into this file. | Yes |
| I did not copy code from another person. | Yes |
| If I received human help, I disclosed it in this file. | Yes |
| I submitted the final code to the OJ by myself. | Yes |
