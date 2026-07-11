
ใช้ไฟล์นี้เฉพาะเมื่อมีการใช้ AI กับโจทย์ OJ ที่เป็น learning-log-required เท่านั้น

1.ข้อมูล OJ
| Item | Answer |
|---|---|
| OJ problem number/title | oj3022 - Temperature |
| OJ submission ID, if submitted | 549456 |
| OJ status | Passed |

2.เครื่องมือ AI ที่ใช้
เขียนชื่อเครื่องมือ AI ที่ใช้
My answer: Gemini

3.การตรวจสอบนโยบายการใช้ AI ของรายวิชา

ตอบหัวข้อนี้อย่างซื่อสัตย์

หัวข้อนี้ยืนยันว่าคุณได้ทำตาม AI workflow ของรายวิชาก่อนและระหว่างใช้ AI

| Statement | Yes / No / Not Applicable | Short note |
|---|---|---|
| I read the relevant workflow before using AI. | Yes | STUDENT_WORKFLOW_WEB_CHAT.th.md |
| I used `instructions/COURSE_AI_INSTRUCTIONS.md`, `instructions/AGENTS.md`, or manually followed the course AI instructions if the tool did not support custom instructions. | Yes | โดยการคัดลอก Prompt จาก COURSE_AI_INSTRUCTIONS.md ไปให้กับ gemini และเน้นยำอย่างเคร่งครัดว่าให้ปฎิบัติตาม |
| I wrote my own problem understanding before asking AI for help. | Yes | การอธิบายโจทย์จะอยู่ที่ submission.md |
| I wrote my own first plan before asking AI for help. | Yes | แผนแรกของฉันจะอยู่ที่ submission.md |
| I used AI as a coach, reviewer, debugger, or test-case helper, not as a full-answer generator. | Yes | .ใช้ AI เพื่อให้ตรวจสอบว่าโค้ดดั้งเดิมมีจุดบกพร่องรวมไปถึงข้อผิดพลาดที่อาจเกิดขึ้นได้ จากนั้น AI ก็จะให้คำใบ้เพื่อให้นำไปแก้ไขปรับปรุงตัวโค้ดด้วยตัวเอง |

4.ฉันถาม AI ให้ช่วยอะไร

My answer: เพื่อตรวจสอบโค้ดดั้งเดิมในการหาข้อผิดพลาดและ Condition ที่ขาดหายไปของโค้ดดั้งเดิม

5.AI ช่วยให้ฉันสังเกตอะไร

เขียนว่า AI ช่วยให้คุณสังเกตอะไร

My answer: Condition ที่ขาดไป, การเรียกใช้ตัวแปรที่ยังไม่ได้สร้าง (NameError) จากโค้ดดั้งเดิมที่ยาวซึ่งทำให้เกิดความสับสนได้, การทำงานทุกอย่างใน 1 Condition

6.ฉันตรวจสอบหรือแก้อะไรด้วยตนเอง

เขียนว่าหลังจากได้รับความช่วยเหลือจาก AI คุณตรวจสอบ ทดสอบ หรือแก้อะไรด้วยตนเอง

My answer: ฉันปรับปรุงตัวโค้ดดั้งเดิมตามคำแนะนำของ AI ให้ลดข้อผิดพลาดและลดความสับสนในโค้ดที่จะเกิดขึ้นและทดสอบ Testcase ใหม่อีกครั้ง

7.ฉันได้เรียนรู้อะไร

เขียน 2-4 ประโยคเกี่ยวกับสิ่งที่ได้เรียนรู้จากโจทย์นี้และจากกระบวนการใช้ AI ช่วย
ให้เน้นการเรียนรู้ของตนเอง

My answer: การเขียนโปรแกรมไม่ควรทำให้ยาวเกินความจำเป็นและไม่ควรเขียนการทำงานทุกอย่างไว้ใน condition เดียวเพราอาจทำให้เกิดความสับสนในตัวโค้ดได้และการเขียนโค้ดโปรแกรมควรคำนึงถึง case ที่เกิดขึ้นให้ได้มากที่สุดเพื่อที่จะสามารถทำโปรแกรมออกมาได้สมบูรณ์แบบและลดข้อผิดพลาดที่จะเกิดขึ้น

8.คำรับรองของนักศึกษา

| Statement | Yes / No |
|---|---|
| I wrote this reflection in my own words. | Yes |
| This reflection describes my real AI use. | Yes |
| I checked AI's suggestions before using them. | Yes |
| I can explain my final code. | Yes |
| I did not ask AI to write this reflection for me. | Yes |
