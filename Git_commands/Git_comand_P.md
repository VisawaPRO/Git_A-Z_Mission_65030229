# คำสั่ง git ที่ขึ้นต้นด้วยอักษร P

## 1.git pull ดึงข้อมูลบนgithubลงมา
![image](https://github.com/VisawaPRO/Git_A-Z_Mission_65030229/assets/144195555/ac53874f-4013-4d2e-ba5e-2fb76ad57736)

## 2.git push ดัยข้อมูลที่ทำที่คอมขึ้นไปที่github
![image](https://github.com/VisawaPRO/Git_A-Z_Mission_65030229/assets/144195555/53921e40-0e46-49f2-ad3d-33cae4e76f24)

## 3.git pack-refs ตามเนื้อผ้า เคล็ดลับของสาขาและแท็ก (เรียกรวมกันว่าการอ้างอิง) จะถูกจัดเก็บหนึ่งไฟล์ต่อการอ้างอิงในไดเร็กทอรี (ย่อย) ภายใต้ไดเร็กทอรี $GIT_DIR/refs แม้ว่าเคล็ดลับสาขาหลายๆ รายการมักจะได้รับการอัปเดตบ่อยครั้ง แต่แท็กส่วนใหญ่และเคล็ดลับสาขาบางส่วนไม่เคยอัปเดตเลย เมื่อพื้นที่เก็บข้อมูลมีแท็กนับร้อยหรือหลายพันแท็ก รูปแบบหนึ่งไฟล์ต่อการอ้างอิงนี้จะทำให้พื้นที่เก็บข้อมูลเปลืองและทำให้ประสิทธิภาพลดลง

## 4.git prune การดำเนินการนี้จะรัน git fsck --unreachable โดยใช้การอ้างอิงทั้งหมดที่มีอยู่ใน refs/ ซึ่งอาจเป็นทางเลือกด้วยชุดของอ็อบเจ็กต์เพิ่มเติมที่ระบุในบรรทัดคำสั่ง และตัดอ็อบเจ็กต์ที่คลายแพ็กทั้งหมดที่ไม่สามารถเข้าถึงได้จากอ็อบเจ็กต์ส่วนหัวใดๆ เหล่านี้จากฐานข้อมูลอ็อบเจ็กต์ นอกจากนี้ยังตัดอ็อบเจ็กต์ที่คลายแพ็กซึ่งพบในแพ็กด้วยการรัน git prune-packed นอกจากนี้ยังลบรายการออกจาก .git/shallow ที่ไม่สามารถเข้าถึงได้โดยผู้อ้างอิงใดๆ

## 5.git p4 คำสั่งนี้ให้วิธีการโต้ตอบกับที่เก็บ p4 โดยใช้ Git

## 6.git pack-objects อ่านรายการอ็อบเจ็กต์จากอินพุตมาตรฐาน และเขียนไฟล์เก็บถาวรที่แพ็กตั้งแต่หนึ่งไฟล์ขึ้นไปด้วยชื่อฐานที่ระบุลงในดิสก์ หรือไฟล์เก็บถาวรที่แพ็กไปยังเอาต์พุตมาตรฐาน
