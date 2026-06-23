# ระบบคะแนน RDU 2569 — จังหวัดสุรินทร์

ระบบติดตามคะแนนการดำเนินงาน RDU (Rational Drug Use) ทั้ง 17 อำเภอในจังหวัดสุรินทร์

## วิธีรันบนเครื่อง

```bash
npm install
npm run dev
```

## วิธี Deploy ขึ้น GitHub Pages

```bash
npm run deploy
```

เว็บจะขึ้นที่ `https://[username].github.io/rdu-surin/`

## เทคโนโลยีที่ใช้

- React 18 + Vite
- Recharts (กราฟ)
- Google Sheets API (ดึงข้อมูล)
- Google Apps Script (บันทึกข้อมูล)
