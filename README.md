# thai-word-check

สกิลให้ AI ตรวจคำภาษาไทยก่อนเริ่ม implement โดยใช้คำที่ระบบใช้อยู่แล้วเป็นหลัก ใช้ได้กับทุกโปรเจกต์ ไม่จำกัดงานการเงิน

## ติดตั้ง

ใช้ทุกโปรเจกต์: คัดลอก `thai-word-check/` ไปไว้ที่ `~/.claude/skills/thai-word-check/`
ใช้เฉพาะโปรเจกต์เดียว: คัดลอกไปที่ `<โฟลเดอร์โปรเจกต์>/.claude/skills/thai-word-check/`

```bash
mkdir -p ~/.claude/skills && cp -r thai-word-check ~/.claude/skills/
```

## ใช้งาน

พิมพ์ "เช็คคำไทยก่อนทำหน้าตั้งค่า" หรือเรียก `/thai-word-check` AI จะค้นคำในระบบ ตัดสินใจ รายงานตาราง "คำที่ใช้ → ที่มา" แล้วค่อย implement

## โครงสร้าง

- `thai-word-check/SKILL.md` — ขั้นตอนหลัก
- `thai-word-check/references/glossary.md` — คำกลางทุกโปรเจกต์ คำพ้อง รูปแบบ
- `thai-word-check/references/projects/` — `_template.md` สำหรับสร้าง glossary ใน repo ของโปรเจกต์ใหม่ และที่วางไฟล์ตัวอย่างโปรเจกต์ `<ชื่อโปรเจกต์>.md` ของคุณเอง (อ่านอย่างเดียว ไม่บังคับ)
- `thai-word-check/references/checklist.md` — เช็กลิสต์ 10 ข้อ
- `thai-word-check/references/message-patterns.md` — แม่แบบข้อความ
