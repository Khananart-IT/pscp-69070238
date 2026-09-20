## 1.ข้อมูล OJ

หมายเลข/ชื่อโจทย์ OJ: oj3477 - Pad Thai

OJ submission ID ถ้ามีการส่งแล้ว: 659362

สถานะ OJ: Passed

เวลาที่ใช้คิดและทำโจทย์ด้วยตนเอง: 1-3 hours

## 2.ความเข้าใจโจทย์ของฉัน

อธิบายโจทย์: โจทย์นี้จะให้สร้างโปรแกรมการทำผัดไทยโดยต้องตรวจสอบว่าวัตถุดิบสำหรับทำผัดไทยว่ามีครบตามที่ต้องการหรือ
ไม่,มีวัตถุดิบอย่างอื่นที่ไม่ได้กำหนดมาไหม, รสชาติมีครบตามที่ต้องการไหม, มีรสชาติอื่นๆด้วยหรือเปล่า

Input: 

    หลายบรรทัด: วัตถุดิบ
    (รับมาเรื่อยๆจนกว่าจะเป็นคำว่า "Cook")
    หลายบรรทัดต่อมา: รสชาติของผัดไทย
    (รับมาเรื่อยๆจนกว่าจะเป็นคำว่า "End")

Output: 

    เป็น 1 ในข้อความดังนี้
    ("This is bad!", "This is not Pad Thai!!!", "Not Bad...", "Delicious!")

Constraints: 

ถ้าใช้วัตถุดิบในการทำผัดไทยไม่ครบจะแสดงผลว่า "This is bad!" ทันทีโดยไม่สนรสชาติ
ถ้าใช้วัตถุดิบในการทำผัดไทยครบตามที่กำหนดแต่รสชาติยังไม่ครบหรือมีรสอื่น จะแสดงผลว่า "Not Bad..."
ถ้าใช้วัตถุดิบที่ไม่ได้กำหนดจะแสดงผลทันทีว่า "This is not Pad Thai!!!" โดยไม่สนรสชาติ
ต้องใช้วัตถุดิบครบและมีรสชาติครบตามที่กำหนดถึงจะแสดงผลว่า "Delicious!"

## 3.แผนแรกของฉัน

ขั้นแรก: กำหนดวัตถุดิบที่ค้องใช้และรสชาติที่ต้องการ

ขั้นที่สอง: รับค่าของวัตถดิบมาถ้าวัตถุดิบไม่ได้อยู่ในที่กำหนดไว้ให้แสดงผล "This is not Pad Thai!!!" (รับจนกว่าจะรับค่า "Cook") ถ้าวัตถุดิบทุกอย่างอยู่ในที่กำหนดไปขั้นตอนต่อไป

ขั้นที่สาม: คำนวณว่าใช้วัตถุดิบครบหรือไม่หากไม่, ให้แสดงผล "This is bad!" และจบการทำงาน ถ้าใช่ไปขั้นตอนต่อไป

ขั้นที่สี่: รับค่าของรสชาติผัดไทยมาถ้ารสชาติไม่อยู่ในที่กำหนดหรือรสชาติไม่ครบให้แสดงผลว่า "Not Bad..."

ขั้นที่ห้า: ถ้าผ่านขั้นตอนทั้งหมดให้แสดงผลว่า "Delicious!"

## 4.วิธีสุดท้ายที่ใช้จริง:
วิธีสุดท้ายของฉันเหมือนกับวิธีแรก
## 5.การทดสอบของฉัน

### Case 1

ทำไมเลือก case นี้: จำนวนวัตถุดิบไม่ครบจะแสดงผลอย่างไร

Input: 

    Egg
    Cook
    Sweet
    Sour
    Salty
    End

Expected output: 

    This is bad!

Actual output: 

    This is bad!

Result: Pass

### Case 2

ทำไมเลือก case นี้: ถ้าวัตถุดิบครบและได้รสชาติที่ต้องการจะเกิดอะไรขึ้น

Input:

    Pad Thai Sauce
    Tofu
    Egg
    Pickle Turnip
    Oil
    Lime
    Shrimp
    Chives
    Bean Sprouts
    Noodle
    Peanuts
    Cook
    Sweet
    Sour
    Salty
    End

Expected output: 

    Delicious!

Actual output: 

    Delicious!

Result: Pass

### Case 3

ทำไมเลือก case นี้: ถ้ามีวัตถุที่ไม่ต้องการและรสชาติอื่นๆจะเป็นอย่างไร

Input: 

    KFC
    Bread
    Potato
    Cook
    Salty
    Spicy
    Plain
    End

Expected output: 

    This is not Pad Thai!!!

Actual output: 

    This is not Pad Thai!!!

Result: Pass

## 6.การใช้ AI
ใช้ AI กับโจทย์นี้หรือไม่: No

## 7.ความช่วยเหลือจากคน / การร่วมมือ
ได้ถามเพื่อน TA ผู้สอน หรือบุคคลอื่นเพื่อขอความช่วยเหลือในโจทย์นี้หรือไม่: No

ใครช่วยคุณ: ไม่มีใคร

ช่วยเหลือแบบใด: ไม่ได้รับความช่วยเหลือจากคน

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
