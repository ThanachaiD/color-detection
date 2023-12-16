# color-detection



Output 

ดับเบิ้ลคลิกสีในรูปภาพ ค่าสีจะแสดงออกมา

![0](https://github.com/ThanachaiD/color-detection/assets/148684074/0d836243-3439-453d-a0b8-5c5e2f96b723)


Data ที่ใช้ทดสอบ

ใช้ข้อมูลสีจากไฟล์ CSV ที่ชื่อ "colors.csv" เพื่อทดสอบ ไฟล์ CSV มีคอลัมน์ที่ระบุข้อมูลเกี่ยวกับสีและค่า RGB ดังนี้

1."color": สีที่ระบุ

2."color_name": ชื่อสี

3."hex": รหัสสี Hexadecimal

4."R": ค่าสีแดง (Red)

5."G": ค่าสีเขียว (Green)

6."B": ค่าสีน้ำเงิน (Blue)


อธิบายโค้ด


![1](https://github.com/ThanachaiD/color-detection/assets/148684074/e3f1899e-70ce-490a-acd5-8eb267237663)

cv2 สำหรับการประมวลผลภาพ , numpy สำหรับการดำเนินการทางตัวเลข , pandas สำหรับการจัดการข้อมูล ,argparse เพื่อจัดการคำสั่งจากคอมมานด์ไลน์

![2](https://github.com/ThanachaiD/color-detection/assets/148684074/bd936327-2246-426b-8650-397b2f9d8461)

ใช้ argparse ในการแปลงอาร์กิวเมนต์ที่ป้อนผ่านคอมมานด์ไลน์


![3](https://github.com/ThanachaiD/color-detection/assets/148684074/360a2201-a983-4ac0-bcc8-23ab868e0968)

อ่านรูปภาพโดย opencv


![4](https://github.com/ThanachaiD/color-detection/assets/148684074/ac41276e-e293-4153-aad5-59073d0476e6)

ตัวแปรที่ใช้เก็บข้อมูลเกี่ยวกับสีที่เลือก และอ่านไฟล์ CSV ที่มีข้อมูลสีโดยใช้ Pandas


![5](https://github.com/ThanachaiD/color-detection/assets/148684074/7a61c739-f363-43d8-9235-8500fc325489)

getColorName คำนวณชื่อสีจากรายการ RGB และ draw_function จัดการกับการดับเบิลคลิกเมาส์เพื่อรับค่าRGB


![6](https://github.com/ThanachaiD/color-detection/assets/148684074/7774f146-0004-408f-aa3d-cf46e0502f04)

ลูป แสดงสี , แสดงข้อมูลสี , หยุดลูปเมื่อกด ESC
