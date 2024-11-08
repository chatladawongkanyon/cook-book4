## ควบคุมการเปิด/ปิด LED ด้วยการกด Switch
1.เปิด VS Code และใช้คำสั่ง Create ESP-IDF Project เลือกโปรเจ็กต์ประเภท blink

<img width="829" alt="image" src="https://github.com/user-attachments/assets/86b97d20-941a-4435-ada4-4278225f8174">

2.การเชื่อมต่อ
การเชื่อมต่อ LED และ Switch เข้ากับ GPIO ของ ESP32
เชื่อมต่อ ขา Anode ของ LED กับ GPIO2 ของ ESP32
เชื่อมต่อ ขา 1 ของ Switch ไปยัง GPIO12 ของ ESP32
เชื่อมต่อ ขา 2 ของ Switch ไปยัง GND ของ ESP32

3.โค้ดนี้ใช้การควบคุม LED โดยใช้สวิตช์ ซึ่งจะอ่านค่าจาก GPIO ที่เชื่อมต่อกับ Switch หากมีการกด Switch ก็จะเปิดหรือปิด LED ตามลำดับ

![Screenshot 2024-11-09 022257](https://github.com/user-attachments/assets/4399f707-87ab-4fe5-a79b-e7054adde9ee)

![Screenshot 2024-11-09 022318](https://github.com/user-attachments/assets/687013d9-53f7-41f7-ae7a-ed4db84637f3)

4.คอมไพล์และอัปโหลดโค้ดไปยัง ESP32
Build, Flash and Monitor เพื่อคอมไพล์และอัปโหลดโค้ดไปยัง ESP32
เมื่อโปรแกรมทำงาน หากกด Switch LED จะเปิดขึ้น
หากปล่อย Switch LED จะปิดลง
ข้อความที่บันทึกไว้ใน Serial Monitor จะบอกสถานะของ Switch และ LED เช่น "Switch is pressed! LED ON" หรือ "Switch is not pressed! LED OFF."
