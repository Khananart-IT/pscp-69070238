## 1.ข้อมูล OJ

หมายเลข/ชื่อโจทย์ OJ: oj3537 - Impostor

OJ submission ID ถ้ามีการส่งแล้ว: 669160

สถานะ OJ: Passed

เวลาที่ใช้คิดและทำโจทย์ด้วยตนเอง: 30-60 minutes

## 2.ความเข้าใจโจทย์ของฉัน

อธิบายโจทย์: โจทย์นี้จะให้สร้างโปรแกรมรับค่าชื่อผู้เล่น, บทบาทของแต่ละคนในเกม AMOGUS และรับค่าชื่อผู้เล่นที่ถูกโหวตออกไปและแสดงผลว่าผลสุดท้ายยังมี impostor เหลือกี่คน, ชื่อผู้เล่น, บทบาทของผู้เล่นที่ยังรอดชีวิตและชื่อผู้เล่น, บทบาทของผู้เล่นที่ถูกโหวตออกแล้ว

Input: 

    รับค่าของชื่อผู้เล่น, บทบาทผู้เล่นมาเรื่อยๆจนกว่าจะเป็นคำว่า Start
    รับค่าของชื่อผู้เล่นที่ถูกโหวตออก (รับเรื่อยๆจนกว่าจะเป็นคำว่า End)
 
Output: 

    บรรทัดที่ 1 จำนวน Impostor ที่ยังเหลือรอด
    หลายบรรทัด แสดงชื่อผู้เล่นและบทบาทของผู้เล่นที่ยังรอด
    หลายบรรทัดอีกที แสดงชื่อผู้เล่นและบทบาทของผู้เล่นที่โดนโหวตออกแล้ว

Constraints: การรับชื่อผู้เล่น, บทบาทของแต่ละคนในเกม AMOGUS ตอนเริ่มจะให้มาในรูปแบบที่คล้ายๆ dict แต่ไม่ใช่ dict ดังนั้นต้อง
แปลงข้อมูลนั้นให้เป็น dict ก่อน

## 3.แผนแรกของฉัน

ขั้นแรก: import json เพื่อแปลง string ในรูปแบบที่คล้ายๆ dict ให้กลายเป็น dict ก่อน

ขั้นที่สอง: รับค่าของชื่อผู้เล่น, บทบาทผู้เล่นมาเรื่อยๆจนกว่าจะเป็นคำว่า Start และเก็บค่าเอาไว้ใน dict ชื่อ PLAYER 

ขั้นที่สาม:  รับค่าของชื่อผู้เล่นที่ถูกโหวตออก (รับเรื่อยๆจนกว่าจะเป็นคำว่า End) และเก็บค่าเอาไว้ใน dict ชื่อ ded_player และลบค่าผู้เล่นนั้นใน PLAYER ออก

ขั้นที่สี่: นำ PLAYER, ded_player มาจัดเรียงตามลำดับตัวอักษรโดยเป็น dict ชื่อ sorted_player และ sorted_ded ตามลำดับ

ขั้นที่ห้า: นับค่าของ Impostor ใน sorted_player , แสดงแสดงชื่อผู้เล่นและบทบาทของผู้เล่นที่ยังรอดและแสดงชื่อผู้เล่นและบทบาทของผู้เล่นที่โดนโหวตออกแล้ว


## 4.วิธีสุดท้ายที่ใช้จริง:
วิธีสุดท้ายของฉันมีเหมือนกับวิธีแรก

### Case 1

ทำไมเลือก case นี้: ถ้าไม่มีผู้เล่นเลยจะเป็นอย่างไร

Input: 

    Start
    End

Expected output:

    0 Impostor Remains
    ***Alive***
    ***Dead***

Actual output: 

    0 Impostor Remains
    ***Alive***
    ***Dead***

Result: Pass

### Case 2

ทำไมเลือก case นี้: ถ้าผู้เล่นทั้งหมดเป็น impostor จะเป็นอย่างไร

Input: 

    {"Hehe" : "Impostor"}
    {"Boi" : "Impostor"}
    {"GGEZ" : "Impostor"}
    {"Yolo" : "Impostor"}
    {"MMMMM" : "Impostor"}
    {"popop" : "Impostor"}
    Start
    popop
    GGEZ
    MMMMM
    End

Expected output: 

    3 Impostor Remains
    ***Alive***
    Boi : Impostor
    Hehe : Impostor
    Yolo : Impostor
    ***Dead***
    GGEZ : Impostor
    MMMMM : Impostor
    popop : Impostor

Actual output: 

    3 Impostor Remains
    ***Alive***
    Boi : Impostor
    Hehe : Impostor
    Yolo : Impostor
    ***Dead***
    GGEZ : Impostor
    MMMMM : Impostor
    popop : Impostor

Result: Pass

### Case 3

ทำไมเลือก case นี้: ถ้าผู้เล่นโดนโหวตออกหมดจะเป็นอย่างไร

Input: 

{"W" : "Crewmate"}
{"B" : "Crewmate"}
{"G" : "Impostor"}
{"Y" : "Crewmate"}
Start
W
B
G
Y
End

Expected output:

    0 Impostor Remains
    ***Alive***
    ***Dead***
    B : Crewmate
    G : Impostor
    W : Crewmate
    Y : Crewmate

Actual output:

    0 Impostor Remains
    ***Alive***
    ***Dead***
    B : Crewmate
    G : Impostor
    W : Crewmate
    Y : Crewmate

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
