# Lab 03 คำตอบ
ชื่อ-สกุล: ...  รหัสนักศึกษา: ...

## Q0
git version 2.56.0.windows.4
user.name=oraya sooknit
user.email=oraya.s@rmutsv.ac.th
init.defaultbranch=main
pull.rebase=false
core.editor=code --wait 


## Q1.1 ... Q5.2
Q1.1 b = 7 เพราะแพตช์เก็บแค่ส่วนต่าง (-b = 5, +b = 7) เมื่อนำไปใช้กับสำเนาของไฟล์เดิม คำสั่ง patch จะเปลี่ยนบรรทัดนั้น ไฟล์จึงกลายเป็นเวอร์ชันใหม่
Q1.2
•	คัดลอกไฟล์: เปลืองพื้นที่ (อาจถึง 100 × 50 = 5,000 ไฟล์ทั้งที่แก้ไม่กี่บรรทัด) หรือสับสนว่าไฟล์ไหนล่าสุดและต่อยอดจากไฟล์ไหน
•	แพตช์: ต้องเก็บ 50 แพตช์และใช้ให้ถูกลำดับ ถ้าแพตช์ชุดใดหาย เวอร์ชันหลังจากนั้นประกอบกลับไม่ได้
•	ใครบอกได้ว่าแก้เพราะอะไร: ไม่มีระบบใดบันทึกไว้ ต้องอาศัยความจำของคนแก้หรือเดาจากชื่อไฟล์ VCS แก้ปัญหานี้ด้วย commit message, ผู้แก้ และเวลา
•	ตอบว่า "คนที่แก้ไฟล์" อย่างเดียวได้ครึ่ง ต้องระบุว่าไม่มีหลักฐานบันทึกไว้จึงได้เต็ม

## Q6.1 ผล git log --oneline --graph --all --decorate
git log --oneline --graph --all --decorate >> LAB03_ANSWERS.md

## Q6.2
(คำตอบ)* 581db50 (HEAD -> main, origin/main, origin/HEAD) docs: เพิ่มคำตอบ Lab 03
*   c7f22f8 Merge branch 'main' of https://github.com/dowadeedao/devops-lab03-65810009
|\  
| * f804072 feat: เพิ่มฟังก์ชัน power (จากเครื่อง B)
* | 3719ad6 docs: ระบุเวอร์ชันล่าสุดใน README (จากเครื่อง A)
|/  
*   2a2bead (tag: v1.1.0) Merge branch 'fix/title'
|\  
| * ebebe83 docs: เปลี่ยนชื่อเป็น Simple Calculator
* | e29f642 docs: เปลี่ยนชื่อเป็น Python Calculator
|/  
*   faec468 Merge branch 'feature/divide'
|\  
| * a56c52b feat: เพิ่มฟังก์ชัน divide
* | f74a867 docs: เพิ่มชื่อผู้จัดทำ
|/  
* 79e4663 feat: เพิ่มฟังก์ชัน multiply พร้อมเทสต์
* 50446d4 Revert "refactor: ปรับปรุง subtract"
* da17a5d refactor: ปรับปรุง subtract
* d65ad0d (tag: v1.0.0) docs: เพิ่มวิธีรันเทสต์ใน README
* 6966adf test: เพิ่ม unit test และ .gitignore
* a2973d0 feat: เพิ่มฟังก์ชัน add และ subtract
