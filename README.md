# LifeSync – Personal Life Management System

> **Organize Your Life, One Day at a Time.**[cite: 1]  
> 🏆 **1st Place Winner – College Mini Project Showcase**

🔗 **Live Demo:** [https://life-sync-nine-pearl.vercel.app](https://life-sync-nine-pearl.vercel.app)[cite: 17]

---

## My Contributions & Architecture Role

This repository is my personal deployment and fork of our 8-member collaborative capstone mini-project. As the project architect and lead contributor for the core entry and habit workflows, my specific contributions include:

- **System Architecture & Prompt Engineering:** Designed the modular folder architecture (`src/modules/`) and isolated prompt specifications for an 8-developer parallel workflow, enabling all teammates to develop on independent Git branches and merge cleanly without conflicts.
- **Landing & Authentication System:** Built the responsive entry Landing Page and client-side Sign Up / Login authentication flow using `localStorage`-based session management (`lifesync_user`).
- **Module 2 – Habit Tracker:** Engineered daily and weekly habit creation, automated current/best streak calculations, and interactive 7-day and 30-day visual consistency grids (`lifesync_habits`)[cite: 3].
- **Recognition:** Awarded **1st Place** at the College Mini Project Showcase.

---

## Project Overview

**LifeSync** is a unified, web-based personal productivity and wellness workspace that brings daily planning, habit building, journaling, mood tracking, and analytics into one seamless interface[cite: 1, 2]. Instead of switching across disconnected tools, all 8 modules synchronize in real time through shared client-side `localStorage` data pipelines[cite: 2, 12].

### Tech Stack
- **Frontend:** React.js (Vite)[cite: 14]
- **Styling & Icons:** Tailwind CSS & Lucide React[cite: 14]
- **Data Visualization:** Recharts[cite: 14]
- **Data Persistence:** Browser `localStorage` (zero-latency client-side storage)[cite: 14]
- **Deployment & Version Control:** Vercel, Git & GitHub (branch-per-module workflow)[cite: 14, 17]

---

## Eight Independent Modules

| Module | Feature Scope | Storage Key |
| :--- | :--- | :--- |
| **1. Goal Management** | Create personal milestones, set target dates, and track 0–100% completion progress[cite: 2]. | `lifesync_goals` |
| **2. Habit Tracker** *(My Module)* | Build daily/weekly habits, toggle daily check-ins, track streaks, and view 7/30-day history grids[cite: 3]. | `lifesync_habits` |
| **3. Task Management** | Organize daily tasks with priority tags (High/Medium/Low), deadlines, and status filters[cite: 3]. | `lifesync_tasks` |
| **4. Calendar Management** | Interactive monthly/weekly views displaying personal events alongside synced task deadlines[cite: 3, 4]. | `lifesync_events` |
| **5. Digital Journal** | Distraction-free personal diary with dated entries, tags, and keyword search[cite: 4]. | `lifesync_journal` |
| **6. Mood Tracker** | Daily emoji check-ins, context notes, mood logs, and distribution charts[cite: 4, 5]. | `lifesync_moods` |
| **7. Reminder Management** | Time-scheduled alerts categorizing Upcoming, Due/Overdue, and Completed reminders[cite: 5]. | `lifesync_reminders` |
| **8. Analytics & Reports** | Cross-module KPI summary cards, weekly reports, and monthly productivity charts[cite: 6]. | *Aggregates all keys* |

---

## Running Locally

```bash
# Clone the repository
git clone [https://github.com/nivimohan/LifeSync.git](https://github.com/nivimohan/LifeSync.git)

# Navigate to the project folder
cd LifeSync

# Install dependencies
npm install

# Start the development server
npm run dev
