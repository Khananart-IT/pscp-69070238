## 1.ข้อมูล OJ

หมายเลข/ชื่อโจทย์ OJ: oj3476 - CuteCat CuteFox

OJ submission ID ถ้ามีการส่งแล้ว: 659277

สถานะ OJ: Passed

เวลาที่ใช้คิดและทำโจทย์ด้วยตนเอง: 1-3 hours

## 2.ความเข้าใจโจทย์ของฉัน

อธิบายโจทย์: โจทย์นี้จะให้สร้างโปรแกรมตรวจสอบว่ามีจำนวนแมวและจำนวนหมาจิ้จอกอยู่ในฝูงกี่ตัวรวมไปถึงแสดงชื่อและหมายเลขของแมวหรือหมาจิ้งจอกตัวนั้น

Input: 

    1.จำนวนแมวรวมกับหมาจิ้งจอกทั้งหมดในฝูง
    2 - จนกว่าจะหมด ชื่อและหมายเลขของแมวหรือหมาจิ้งจอกตัวนั้น

Output: 

    1.จำนวนแมวในฝูง
    2.จำนวนหมาจิ้งจอกในฝูง
    3 - ไปเรื่อยๆ ชื่อแมว, หมายเลขแมว, ชื่อหมาจิ้งจอก, หมายเลขหมาจิ้งจอก(โดยแมวจะแสดงผลก่อนหมาจิ้งจอก)

Constraints: 

ถ้าในฝูงไม่มีหมายเลข "Cat01" ให้เพิ่มแมวชื่อ "Garfield" ที่มีหมายเลข "Cat01" เข้าไปในฝูงและถ้าในฝูงไม่มีหมายเลข "Fox01" ให้เพิ่มหมาจิ้งจอกชื่อ "Fubuki" ที่มีหมายเลข "Fox01" เข้าไป
(แต่ถ้ามีชื่อ 2 ตัวนี้อยู่ในหมายเลขอื่นแล้วไม่ต้องทำอะไร)

## 3.แผนแรกของฉัน

ขั้นแรก: รับค่าของจำนวนแมวรวมกับหมาจิ้งจอกทั้งหมดในฝูง

ขั้นที่สอง: รับค่าชื่อและหมายเลขของแมวและหมาจิ้งจอกแต่ละตัวและเก็บไว้ใน dict

ขั้นที่สาม: นับจำนวนแมวและหมาจิ้งจอกใน dict นั้น

ขั้นที่สี่: แสดงชื่อของแมว,หมายเลขของแมว,ชื่อของหมาจิ้งจอก,หมายเลขของหมาจิ้งจอก

## 4.วิธีสุดท้ายที่ใช้จริง:
วิธีสุดท้ายของฉันมีพื้นฐานจากวิธีแรกแต่เพิ่มขั้นตอนที่ถ้าในฝูงนั้นไม่มีหมายเลข "Cat01" ให้เพิ่มแมวชื่อ "Garfield" ที่มีหมายเลข "Cat01" เข้าไปในฝูงและถ้าในฝูงไม่มีหมายเลข "Fox01" ให้เพิ่มหมาจิ้งจอกชื่อ "Fubuki" ที่มีหมายเลข "Fox01" เข้าไป
## 5.การทดสอบของฉัน

### Case 1

ทำไมเลือก case นี้: ถ้าไม่มีจำนวนแมวรวมกับหมาจิ้งจอกในฝูงเลยจะเป็นอย่างไร

Input: 

    0

Expected output: 

    Cat : 1
    Fox : 1
    Garfield : Cat01
    Fubuki : Fox01

Actual output: 

    Cat : 1
    Fox : 1
    Garfield : Cat01
    Fubuki : Fox01

Result: Pass

### Case 2

ทำไมเลือก case นี้: ถ้า Garfield เป็นแมวตัวอื่นไปแล้วจะเป็นอย่างไร

Input:

    5
    {"Chi" : "Cat06"}
    {"Tom" : "Cat05"}
    {"Garfield" : "Cat04"}
    {"Shiro" : "Fox02"}
    {"Senko" : "Fox10"}

Expected output: 

    Cat : 3
    Fox : 3
    Garfield : Cat04
    Tom : Cat05
    Chi : Cat06
    Fubuki : Fox01
    Shiro : Fox02
    Senko : Fox10

Actual output: 

    Cat : 3
    Fox : 3
    Garfield : Cat04
    Tom : Cat05
    Chi : Cat06
    Fubuki : Fox01
    Shiro : Fox02
    Senko : Fox10

Result: Pass

### Case 3

ทำไมเลือก case นี้: ถ้า Fubuki เป็นแมวแทนจะเป็นอย่างไร

Input: 

    7
    {"Fubuki" : "Cat55"}
    {"Shiro" : "Fox01"}
    {"Garfield" : "Fox06"}
    {"Kin" : "Cat05"}
    {"Okayu" : "Cat63"}
    {"Kuro" : "Fox02"}
    {"Tom" : "Cat07"}

Expected output: 

    Cat : 4
    Fox : 3
    Kin : Cat05
    Tom : Cat07
    Fubuki : Cat55
    Okayu : Cat63
    Shiro : Fox01
    Kuro : Fox02
    Garfield : Fox06

Actual output: 

    Cat : 4
    Fox : 3
    Kin : Cat05
    Tom : Cat07
    Fubuki : Cat55
    Okayu : Cat63
    Shiro : Fox01
    Kuro : Fox02
    Garfield : Fox06

Result: Pass

## 6.การใช้ AI
ใช้ AI กับโจทย์นี้หรือไม่: Yes

## 7.ความช่วยเหลือจากคน / การร่วมมือ
ได้ถามเพื่อน TA ผู้สอน หรือบุคคลอื่นเพื่อขอความช่วยเหลือในโจทย์นี้หรือไม่: Yes

ใครช่วยคุณ: Google

ช่วยเหลือแบบใด: การใช้ json ที่สามารถใช้กับ dict ได้เช่นกันนอกจาก list รวมไปถึงการเรียงลำดับด้วย value ผ่านการใช้ lambda

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
