แก้ไขไฟล์ README.md ให้มีเนื้อหาพื้นฐาน (CI badge จะเพิ่มใน Part 4):

README.mdCopy
# TaskBoard — ระบบจัดการงาน

![CI](https://github.com/faymori/taskboard/actions/workflows/ci.yml/badge.svg)

ระบบ CRUD สำหรับจัดการงาน สร้างด้วย Express.js + PostgreSQL + Vue 3

## Tech Stack
- **Backend:** Node.js + Express.js + PostgreSQL
- **Frontend:** Vue 3 + Vite
- **Container:** Docker + Docker Compose
- **CI/CD:** GitHub Actions

## วิธีรัน (Local)
```bash
# Clone
git clone https://github.com/faymori/taskboard.git
cd taskboard

# รัน ด้วย Docker Compose
docker compose up --build
```
เข้า http://localhost เพื่อดู Frontend

## API Endpoints
| Method | Path | คำอธิบาย |
|--------|------|----------|
| GET | /health | Health check |
| GET | /api/tasks | ดึงงานทั้งหมด |
| POST | /api/tasks | สร้างงานใหม่ |
| PUT | /api/tasks/:id | แก้ไขงาน |
| DELETE | /api/tasks/:id | ลบงาน |