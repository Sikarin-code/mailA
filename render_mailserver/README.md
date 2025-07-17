
# Render Mail Server + Webmail (รับเมลเท่านั้น)

## ใช้สำหรับ:
- รับ OTP / อีเมลยืนยันจาก TikTok
- เข้าดูเมลผ่าน Webmail (Roundcube)

## วิธีใช้งาน
1. push โฟลเดอร์นี้ขึ้น GitHub
2. สร้าง 2 Web Service บน Render
   - mail (internal, ไม่เปิด public)
   - webmail (PORT: 8080)
3. ตั้ง DNS:
   - A: mail.livepro.app → Render Webmail IP
   - MX: @ → mail.livepro.app (Priority 10)
4. เข้าที่: http://mail.livepro.app/webmail
   Login: info@livepro.app / Test1234
