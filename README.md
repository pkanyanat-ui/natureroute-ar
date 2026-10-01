# หน้า AR ส่องสัตว์ (แยกจาก Wix)

หน้าเว็บชุดนี้แสดงโมเดล 3D และเปิด AR ได้ทั้ง iPhone (Quick Look) และ Android (Scene Viewer / WebXR)
โดยใช้ไฟล์โมเดลเดิมที่เก็บอยู่บน Wix ไม่ต้องอัปโหลดโมเดลใหม่

- `index.html` หน้าเลือกโซน
- `reservoir.html`, `thaplan.html`, `pangsida.html` หน้าโซน
- `animals/*.html` หน้าสัตว์ 21 หน้า (1 หน้าต่อ 1 ตัว)
- `pages.csv` รายการหน้าและไฟล์โมเดลทั้งหมด ใช้ทำ QR code

## วิธีขึ้นเว็บด้วย GitHub Pages (ฟรี)
1. สมัคร/เข้าสู่ระบบ github.com แล้วกด New repository ตั้งชื่อ เช่น `natureroute-ar` เลือก Public
2. กด "uploading an existing file" แล้วลากไฟล์และโฟลเดอร์ทั้งหมดในโฟลเดอร์นี้ขึ้นไป กด Commit
3. ไปที่ Settings → Pages → Source: Deploy from a branch → Branch: main / (root) → Save
4. รอ 1–2 นาที จะได้ลิงก์ `https://<ชื่อผู้ใช้>.github.io/natureroute-ar/`

## เชื่อมกับ Wix
ในหน้าแผนที่ "ส่องสัตว์ด้วย AR" บน Wix ให้แต่ละโซนลิงก์ไปที่หน้าโซนใหม่
(เช่น `.../natureroute-ar/reservoir.html`) หรือทำปุ่ม/QR code ไปที่หน้าสัตว์แต่ละตัว

## ข้อควรรู้เวลาใช้งาน
- iPhone ต้องเปิดใน **Safari** โดยตรง ถ้าเปิดลิงก์จากในแอป LINE / Facebook / Instagram ปุ่ม AR จะไม่ทำงาน
  (ให้กด "เปิดใน Safari" ก่อน)
- Android ใช้ Chrome และเครื่องต้องรองรับ Google Play Services for AR
- โมเดลบางตัวใหญ่ (หมูป่า 24 MB, กวางป่าโซนทับลาน 15 MB) ควรใช้ Wi-Fi
