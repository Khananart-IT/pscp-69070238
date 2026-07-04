1.ข้อมูล OJ

หมายเลข/ชื่อโจทย์ OJ: oj2996

OJ submission ID ถ้ามีการส่งแล้ว: 542351

สถานะ OJ: Passed

เวลาที่ใช้คิดและทำโจทย์ด้วยตนเอง: 15-30 minutes

2.ความเข้าใจโจทย์ของฉัน

อธิบายโจทย์: โจทย์ให้ทำโปรแกรมสลับตัวอักษรภาษาอังกฤษความยาว 5 ตัวอักษรจากหน้าไปหลังเป็นหลังไปหน้าโดยผลลัพธ์ออกมาต้องเป็นตัวพิมพ์เล็ก

Input: ตัวอักษรภาษาอังกฤษยาว 5 ตัวอักษร

Output: ตัวอักษรภาษาอังกฤษยาว 5 อักษรแบบกลับด้านเป็นตัวพิมพ์เล็ก

Constraints: หากตัวอักษรที่รับเข้ามาเป็นตัวพิมพ์ใหญ่ต้องเปลี่ยนให้เป็นตัวพิมพ์เล็ก
ก่อนจึงจะนำไปกลับด้าน

3.แผนแรกของฉัน

ขั้นแรก: สร้าง input เพื่อรับค่าของตัวอักษรภาษาอังกฤษความยาว 5 ตัวอักษร

ขั้นที่สอง: แปลงตัวอักษรที่รับค่าเข้ามาให้เป็นตัวพิมพ์เล็กทั้งหมด

ขั้นที่สาม: กลับด้านตัวอักษรที่แปลงเป็นตัวพิมพ์เล็กทั้งหมดจากหน้าไปหลังเป็นหลัง
ไปหน้าโดยใช้ <text>[::-1] เพื่อให้ output ออกมาจะเป็นตัวอักษรกลับด้าน

4.วิธีสุดท้ายที่ใช้จริง:
วิธีสุดท้ายจะคล้ายคลึงกับวิธีแรกแต่จะเปลี่ยนเป็นการพิมพ์ตัวอักษรกลับด้านก่อนแล้วจึงทำให้ข้อความเป็น
ตัวพิมพ์เล็กทั้งหมดในบรรทัดเดียว

5.การทดสอบของฉัน

Case 1

ทำไมเลือก case นี้: เป็นตัวอักษรตัวพิมพ์เล็กทั้งหมด

Input: korfg

Expected output: gfrok

Actual output: gfrok

Result: Pass

Case 2

ทำไมเลือก case นี้: เป็นตัวอักษรตัวใหญ่ทั้งหมด

Input: FKQWL

Expected output: lwqkf

Actual output: lwqkf

Result: Pass

Case 3

ทำไมเลือก case นี้: มีทั้งตัวอักษรตัวพิมพ์เล็กและตัวพิมพ์ใหญ่รวมกัน

Input: PvIsD

Expected output: dsivp

Actual output: dsivp

Result: Pass

6.การใช้ AI
ใช้ AI กับโจทย์นี้หรือไม่: No

7.ความช่วยเหลือจากคน / การร่วมมือ
ได้ถามเพื่อน TA ผู้สอน หรือบุคคลอื่นเพื่อขอความช่วยเหลือในโจทย์นี้หรือไม่
No

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
