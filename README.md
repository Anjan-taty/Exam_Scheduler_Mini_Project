# 📚 Exam Scheduler – Intelligent Timetable Generator

An intelligent system that automatically generates **conflict-free exam timetables** using **graph algorithms and optimization strategies**.

Built for **IIIT Dharwad**, this tool eliminates manual scheduling effort and guarantees **zero student conflicts**.

---

## 🎯 Overview

This is a **web-based exam scheduling system** that:

- 📊 Takes student enrollment data (Excel)
- 🧠 Builds a conflict graph
- 🎯 Applies graph coloring
- ⚡ Generates an optimized timetable

💡 **Key Highlight:**  
No hardcoded data — everything is dynamically computed from uploaded files.

---

## 🚀 Key Features

- 🧠 **Conflict-Free Scheduling**
- 📊 **Graph Coloring Algorithm**
- 🔁 **Retry Mechanism for Optimization**
- 📅 **Dynamic Date Allocation**
- 📈 **Real-Time Statistics Dashboard**
- 📥 **Excel Export Support**
- 🌐 **Browser-Based (No Installation)**

---

## 🧠 Core Idea (Visual)

```
Student Enrollments
        ↓
Conflict Graph
        ↓
Graph Coloring
        ↓
Slot Assignment
        ↓
Final Timetable
```

---

## 📊 Version Evolution

### 🟡 Version 1 – Basic Scheduler

| Feature | Status |
|--------|-------|
| Slot Assignment | ✅ |
| Excel Input | ✅ |
| Conflict Detection | ❌ |
| Optimization | ❌ |

---

### 🟢 Version 2 – Intelligent Scheduler ✨

| Feature | Status |
|--------|-------|
| Conflict Detection | ✅ |
| Graph Coloring | ✅ |
| Zero Conflicts | ✅ |
| Retry Mechanism | ✅ |
| Cross-Year Handling | ✅ |
| Student Constraints | ✅ |

---

## ⚙️ How It Works

### 🔄 Pipeline

```
Upload Excel Files
        ↓
Extract Data
        ↓
Build Conflict Graph
        ↓
Apply Graph Coloring
        ↓
Generate Schedule
```

---

## 🧠 Algorithm Details

### 🎨 Graph Coloring

- Each course = Node  
- Edge = Conflict (same student enrolled)  
- Color = Exam Slot  

👉 Goal: Use **minimum colors (slots)** with **no conflicts**

---

### 📊 Complexity

| Metric | Value |
|------|------|
| Time | O(V² + E) |
| Space | O(V + E) |

---

## 📈 Conflict Graph (Concept)

```
Course A ─── Course B
     │          │
     └────── Course C
```

👉 Connected courses cannot be in the same slot

---

## 📊 Scheduling Strategy

| Scenario | Strategy |
|--------|--------|
| More Days Available | Prefer Morning Slots |
| Limited Days | Use Both Slots |
| High Conflicts | Retry + Shuffle |

---

## 🔁 Retry Optimization

```
Attempts ≤ 8
→ Shuffle course order
→ Try new schedule
→ Select best valid solution
```

---

## 📊 Sample Output

### 🗓️ Timetable

```
Date       | 17-02 | 18-02 | 19-02
-----------+-------+-------+-------
FN 11:00AM | CS307 | EC307 | DS308
AN 3:00PM  | CS304 | DA265 | CS266
```

---

### 📊 Enrollment Stats

```
Course Code | Students
------------|---------
CS206       | 171
CS265       | 85
CS307       | 138
```

---

## 📈 System Metrics (Example)

| Metric | Value |
|------|------|
| Courses | 56 |
| Students | 622 |
| Min Slots | 10 |
| Min Days | 5 |
| Conflicts | 0 ✅ |

---

## 🎯 Constraints

### 🔴 Hard Constraints

- ❌ No student has 2 exams in same slot  
- 📚 Same course codes → same slot  
- 🧑 Max 2 exams/day  

---

### 🟢 Soft Constraints

- Prefer 1 exam/day  
- Minimize afternoon usage  
- Minimize total days  

---

## 🛠️ Tech Stack

| Layer | Tech |
|------|-----|
| Frontend | HTML + JS |
| Processing | JavaScript |
| Excel Parsing | SheetJS |
| Algorithm | Graph Theory |

---

## 🚀 Usage Guide

### 1️⃣ Upload Files
- 2nd Year Excel  
- 3rd Year Excel  

---

### 2️⃣ Analyze

Click:
```
🔍 Analyze & Calculate Minimum Days
```

---

### 3️⃣ Add Dates

- Add required number of days  
- Dates auto-sort  

---

### 4️⃣ Generate Timetable

Click:
```
🚀 Generate Timetable
```

---

### 5️⃣ Download

- 📥 Timetable Excel  
- 📥 Enrollment Stats  

---

## 📊 System Behavior (Visual)

```
Normal Case:
Balanced distribution → Efficient schedule ✅

Edge Case:
Heavy conflicts → Retry mechanism activated 🔁
```

---

## 🚀 Future Improvements

- 🏫 Room Allocation  
- 👨‍🏫 Invigilator Assignment  
- 📩 Notification System  
- 🌐 Deployment  
- 🤖 ML-based optimization  

---

## 🏭 Industry Relevance

| Feature | This Project | Industry Systems |
|------|-------------|----------------|
| Scheduling | Graph Coloring | Optimization Engines |
| Conflict Handling | Exact | Heuristic + ML |
| Scale | Hundreds | Millions |

---

## 🎯 Who Can Use This?

- 🎓 Universities  
- 🏫 Colleges  
- 📅 Exam Coordinators  
- 🧠 Algorithm learners  

---

## 👨‍💻 Author

**Anjan (Taty)**  
🚀 AI + Backend + System Design Enthusiast  

---

## ⭐ Support

If you like this project, give it a ⭐ — it really helps!

---

## ❤️ Acknowledgments

- IIIT Dharwad  
- Graph Theory (CS206)  
- SheetJS Library  

---

### 💡 Final Note

> Eliminating scheduling conflicts, one exam at a time.