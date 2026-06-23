# ขั้นตอน Deploy ขึ้น GitHub Pages

## สิ่งที่ต้องมี
- Node.js (nodejs.org)
- Git (git-scm.com)
- บัญชี GitHub

---

## ขั้นตอนที่ 1 — สร้าง Repository บน GitHub

1. เข้า github.com → Login
2. กด **+ → New repository**
3. ตั้งชื่อ: `rdu-surin`
4. เลือก **Public**
5. กด **Create repository**

---

## ขั้นตอนที่ 2 — นำโฟลเดอร์นี้ขึ้น GitHub

เปิด Terminal แล้วรัน (เปลี่ยน YOUR_USERNAME เป็น GitHub username ของคุณ):

```bash
cd rdu-deploy
npm install
git init
git add .
git commit -m "RDU Score System 2569"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/rdu-surin.git
git push -u origin main
```

---

## ขั้นตอนที่ 3 — Deploy

```bash
npm run deploy
```

รอ ~1 นาที แล้วเปิด:
```
https://YOUR_USERNAME.github.io/rdu-surin/
```

---

## ขั้นตอนที่ 4 — เปิด GitHub Pages

1. GitHub repo → **Settings → Pages**
2. Branch: เลือก **gh-pages** → Save
3. รอ 1–2 นาที เว็บพร้อมใช้งาน

---

## อัปเดตเว็บในอนาคต

แก้ไขไฟล์ใน src/ แล้วรัน:
```bash
git add . && git commit -m "update" && git push
npm run deploy
```
