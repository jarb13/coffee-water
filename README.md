# ☕ Coffee Water Lab — คำนวณแร่ธาตุน้ำชงกาแฟ

เว็บแอปพลิเคชันสำหรับคำนวณสัดส่วนและน้ำหนักสารแร่ธาตุผสมน้ำชงกาแฟตามมาตรฐาน **SCA (ppm as CaCO₃)** รองรับทั้งการชั่งผงผสมลงกาดริป/เหยือกโดยตรง และการทำหัวเชื้อใส่ขวดหยด (Dropper Concentrate)

## ✨ ฟีเจอร์หลัก
- **8 โปรไฟล์น้ำสำเร็จรูป (Presets):** เลือกตามโพรเซสกาแฟ (Washed, Natural, Honey, Anaerobic) หรือตามโทนรสชาติที่ต้องการเน้น (Acidity, Sweetness, Body, Balanced SCA)
- **ปรับจูนอิสระ (Custom TDS & Ratios):** กำหนดปริมาณน้ำชงกาแฟ (ml), ค่า TDS เป้าหมาย (ppm) และสัดส่วนแร่ธาตุ 3 ชนิด (Mg, Ca, Buffer) พร้อมคำนวณค่า GH, KH และอัตราส่วน GH:KH อัตโนมัติ
- **คำนวณตามน้ำหนักโมเลกุลจริง:**
  - **Magnesium (Mg):** ดีเกลือฝรั่ง (Epsom Salt - $\text{MgSO}_4\cdot7\text{H}_2\text{O}$) หรือ แมกนีเซียมคลอไรด์ ($\text{MgCl}_2\cdot6\text{H}_2\text{O}$)
  - **Calcium (Ca):** แคลเซียมแลคเตท (Calcium Lactate Pentahydrate / Anhydrous), แคลเซียมคลอไรด์ หรือ ยิปซัม
  - **Buffer (KH/Na):** เบกกิ้งโซดา (Baking Soda - $\text{NaHCO}_3$) หรือ เกลือบริสุทธิ์ ($\text{NaCl}$)
- **2 โหมดแสดงผลลัพธ์:**
  1. **ชั่งผงผสมลงกาดริป/เหยือกโดยตรง** (แสดงผลทั้งหน่วยกรัม `g` และมิลลิกรัม `mg`)
  2. **ผสมหัวเชื้อใส่ขวด Dropper (30 / 50 / 100 ml)** พร้อมตัวเลือกระดับความเข้มข้น 4 ระดับตามลิมิตการละลายน้ำจริง (ไม่ตกผลึกนอนก้นขวด) และสูตรรวมขวดเดียว (All-in-One)

## 🚀 วิธีอัปโหลดขึ้น GitHub และ Deploy ลง Vercel

โปรเจกต์นี้เป็น **Static Web Application** ที่พร้อมใช้งานทันทีโดยไม่ต้องรันคำสั่ง Build ใดๆ

### 1. อัปโหลดขึ้น GitHub
- สร้าง Repository ใหม่บน [GitHub](https://github.com/new)
- อัปโหลดไฟล์ทั้งหมดในโฟลเดอร์นี้ (`index.html`, `favicon.svg`, `vercel.json`, `.gitignore`, `README.md`) ขึ้นไปยัง Repository (ผ่านหน้าเว็บ GitHub **"Add file" -> "Upload files"** หรือผ่าน **GitHub Desktop** / **Git CLI**)

### 2. Deploy ลง Vercel
1. เข้าไปที่ [Vercel Dashboard](https://vercel.com/new) และล็อกอินด้วยบัญชี GitHub
2. กด **Import** โปรเจกต์ Repository ที่เพิ่งสร้าง
3. ตั้งค่าการ Deploy (ปกติระบบจะตรวจจับอัตโนมัติจาก `vercel.json`):
   - **Framework Preset:** `Other`
   - **Build Command:** *(เว้นว่างไว้)*
   - **Output Directory:** *(เว้นว่างไว้)*
4. กดปุ่ม **Deploy** รอประมาณ 5–10 วินาที เว็บไซต์จะพร้อมใช้งานทันที!
