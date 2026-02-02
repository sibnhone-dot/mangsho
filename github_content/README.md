# Mentor App - GitHub Backend

This folder contains all data for your Mentor tutor app. Push this to your GitHub repo: https://github.com/sibnhone-dot/mangsho

## 📁 Folder Structure

```
mangsho/
├── data/                        ← Editable data (like a database)
│   ├── teachers.json           ← Teacher logins
│   ├── students.json           ← Student info
│   ├── schedule_patterns.json  ← Who teaches whom & when
│   ├── holidays.json           ← Holiday dates
│   └── content_index.json      ← Maps chapters to content files
│
└── content/                     ← Teaching content
    ├── c10/physics/motion.json
    ├── c9/math/algebra.json
    └── ...
```

## ✏️ How to Edit Data

1. Go to https://github.com/sibnhone-dot/mangsho
2. Click on any JSON file (e.g., `data/teachers.json`)
3. Click the pencil icon ✏️ to edit
4. Make changes
5. Click "Commit changes"

**Changes go live within 24 hours** (jsDelivr cache). To force refresh, add `?v=2` to URL.

## 📊 Data Formats

### teachers.json
```json
{
  "teachers": [
    {
      "teacher_id": "T001",
      "name": "Rahim Ahmed",
      "phone": "01712345678",
      "password": "rahim123",
      "active": true
    }
  ]
}
```

### students.json
```json
{
  "students": [
    {
      "student_id": "S001",
      "name": "Anik Rahman",
      "class": "Class 10",
      "parent_phone": "01723456789"
    }
  ]
}
```

### schedule_patterns.json
```json
{
  "schedule_patterns": [
    {
      "pattern_id": "P001",
      "teacher_id": "T001",
      "student_id": "S001",
      "student_name": "Anik Rahman",
      "days": ["Mon", "Wed", "Fri"],
      "time": "10:00",
      "class": "Class 10",
      "subject": "Physics",
      "chapter_key": "c10-physics-motion",
      "chapter_name": "Motion and Force",
      "start_date": "2026-02-01",
      "end_date": "2026-12-31"
    }
  ]
}
```

### holidays.json
```json
{
  "holidays": [
    { "date": "2026-02-21", "reason": "National Day" }
  ]
}
```

## 🚀 Capacity

| Metric | Limit |
|--------|-------|
| Requests/month | 50 million |
| Storage | 100GB |
| Users supported | 10,000+ daily |
| Cost | FREE forever |
