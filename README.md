# Postes (เว็บการ์ดไปรษณีย์)

เว็บนี้เป็นไฟล์เดียวจบ: `index.html`
- CSS, JavaScript และรูปทั้งหมด (ตู้ไปรษณีย์ แสตมป์ ซีล พนักงานสกูตเตอร์) ฝังอยู่ในไฟล์นี้แล้ว
- สิ่งเดียวที่โหลดจากภายนอกคือฟอนต์จาก Google Fonts (ต้องมีอินเทอร์เน็ต)
- ไม่ต้องใช้ localhost หรือเซิร์ฟเวอร์ใดๆ

## ขึ้นเว็บด้วย GitHub Pages
1. สมัคร/เข้าสู่ระบบที่ https://github.com
2. กด New repository ตั้งชื่อ เช่น `postes` เลือก Public แล้วกด Create repository
3. กด "uploading an existing file" (หรือ Add file > Upload files) แล้วลากไฟล์ `index.html` (และ `.nojekyll` ถ้าเห็น) ไปวาง
4. กด Commit changes
5. ไปที่ Settings > Pages > Build and deployment > Source เลือก "Deploy from a branch"
   Branch เลือก `main` และโฟลเดอร์ `/ (root)` แล้วกด Save
6. รอประมาณ 1-2 นาที แล้วเปิดที่อยู่เว็บที่ GitHub แสดง
   รูปแบบ: https://ชื่อบัญชี.github.io/postes/

## อัปเดตเว็บทีหลัง
อัปโหลดไฟล์ `index.html` ใหม่ทับของเดิมที่หน้า repository (Add file > Upload files) แล้ว Commit
หลังอัปเดตให้รีเฟรชแรงๆ (Ctrl+Shift+R) หรือรอสักพัก ถ้ายังเห็นของเก่า

## ก่อนเปิดรับลูกค้าจริง
- ตอนนี้เป็นโหมดทดลอง (`const TRIAL=true` ใน index.html): ไม่มีล็อกอิน ไม่มี QR ไม่เก็บเงินจริง
- เลขพร้อมเพย์ในไฟล์ (`PROMPTPAY_ID`) เป็นเลขตัวอย่าง ต้องแก้เป็นของคุณก่อนเปิด QR
- ออเดอร์ส่งจริงยังเก็บในเบราว์เซอร์ของลูกค้า ต้องมีหลังบ้านจริงก่อนเปิดขาย
- ลิงก์จดหมายฝังที่อยู่เว็บไว้ ถ้าเปลี่ยนที่อยู่เว็บภายหลัง ลิงก์เก่าจะเปิดไม่ได้
