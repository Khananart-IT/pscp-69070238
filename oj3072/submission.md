## 1.ข้อมูล OJ

หมายเลข/ชื่อโจทย์ OJ: oj3072 - A-E-I-O-U

OJ submission ID ถ้ามีการส่งแล้ว: 571245

สถานะ OJ: Passed

เวลาที่ใช้คิดและทำโจทย์ด้วยตนเอง: 15-30 minutes

## 2.ความเข้าใจโจทย์ของฉัน

อธิบายโจทย์: โจทย์นี้จะให้สร้างโปรแกรมนับจำนวนสระที่อยู่ในข้อความ โดยไม่สำคัญว่าจะเป็นตัวพิมพ์เล็กหรือตัวพิมพ์ใหญ่

Input: ข้อความจำนวน 1 ถึง 999 ตัวอักษร

Output: แสดงสระที่พบในข้อความและระบุจำนวนสระที่พบโดยเป็น case not sensitive

Constraints: ถ้าไม่พบสระบางสระจะไม่แสดง output ที่เป็นสระนั้นออกมา

## 3.แผนแรกของฉัน

ขั้นแรก: สร้างฟังก์ชันที่ไว้สำหรับคำนวณจำนวนสระที่ text โดยตัวแปร text คือข้อความที่ input เข้ามาและจะปรับเปลี่ยนให้ข้อความ text เป็นตัวพิมพ์เล็กทั้งหมดเพื่อความสะดวกต่อการคำนวณ

ขั้นที่สอง: สร้างตัวแปร a_letter, e_letter, i_letter, o_letter และ u_letter สำหรับเก็บข้อมูลจำนวนสระ

ขั้นที่สาม: สร้าง for loop สำหรับเช็คว่าแต่ละตัวเป็นสระหรือไม่ หากใช่จะทำการเพิ่มจำนวนของสระนั้น

ขั้นที่สี่: เช็คตัวแปร a_letter, e_letter, i_letter, o_letter และ u_letter ว่ามากกว่า 0 ไหม ถ้าใช่จะให้แสดง output ออกมา

## 4.วิธีสุดท้ายที่ใช้จริง:
วิธีสุดท้ายมีพื้นฐานจากวิธีแรกแต่มีการปรับเปลี่ยนโดยให้มีการเช็คตั้งแต่ต้นว่ามีสระนั้นไหม ถ้ามีจะทำการนับจำนวนสระนั้นจากนั้นทำการแสดงสระและจำนวนสระออกมา

## 5.การทดสอบของฉัน

### Case 1

ทำไมเลือก case นี้: ทดสอบว่าถ้าใน text ไม่มีสระเลย ผลจะออกมาเป็นอย่างไร

Input: KFC

Expected output: 

Actual output: 

Result: Pass

### Case 2

ทำไมเลือก case นี้: เช็คว่าหาก สระ e มานำหน้าก่อนสระ a จะแสดงผลออกมาตามที่ต้องการไหม

Input: eAtEat

Expected output: 

        a : 2
        e : 2

Actual output: 

        a : 2
        e : 2

Result: Pass

### Case 3

ทำไมเลือก case นี้: เช็คว่าหากข้อความนี้มีสระทุกสระจะสามารถทำงานได้ตามที่ต้องการไหม

Input: uaeoidfjgitieospfoakdlfkoadsfol

Expected output: 

        a : 3
        e : 2
        i : 3
        o : 5
        u : 1

Actual output: 

        a : 3
        e : 2
        i : 3
        o : 5
        u : 1

Result: Pass

## 6.การใช้ AI
ใช้ AI กับโจทย์นี้หรือไม่: No

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
