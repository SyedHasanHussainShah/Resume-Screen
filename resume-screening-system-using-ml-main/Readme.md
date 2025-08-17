# 📝 Resume Screening Application

A **modern, visually interactive resume screening platform** to help recruiters analyze and compare candidates efficiently.

---

## 🚀 Project Overview

A **React-based** application streamlining the resume screening process by providing:
- 📄 **PDF document uploads** for job descriptions & resumes
- 🤖 **Automated skill matching and scoring**
- 📊 **Visual analytics & demographics**
- 🏆 **Candidate ranking system**
- ✅ **Shortlisting & report generation**

---

## ✨ Features

### 📂 Document Upload
- **Drag-and-drop** interface for job descriptions & resumes
- **Multi-file upload** support for resumes
- 📈 **Progress tracking** for uploads
- ✅ PDF format validation & visual feedback

### 🧠 Analysis & Matching
- **Automated skill extraction & matching**
- **Match score** calculation based on required skills
- **Experience & education** level detection
- **Location-based** grouping

### 📈 Results & Analytics

#### 1. Demographics Dashboard
- 🏅 Experience distribution chart
- 🎓 Education level breakdown
- 🌍 Geographic distribution
- **Key statistics**:
  - Total candidates
  - Average experience
  - Average match score
  - Most common location

#### 2. Candidate Rankings
- **Sorted by match score**
- 🥇🥈🥉 Medal system for top 3 candidates
- Detailed cards showing:
  - Match percentage
  - Found/missing skills
  - Experience details
  - Education & location

#### 3. Shortlisting Features
- **Select candidates** for shortlist
- 📥 **Generate PDF reports** for shortlisted candidates
- **Downloadable summary**

---

## ⚙️ Tech Stack

### Frontend
- [React.js](https://react.dev/)
- [Tailwind CSS](https://tailwindcss.com/) (utility-first styling)
- [Chart.js](https://www.chartjs.org/) (visualizations)
- [PDF-lib](https://pdf-lib.js.org/) (report generation)

### UI Components
- Drag & drop file upload
- Progress bars
- Interactive & responsive charts
- Modal dialogs

### Data Visualization
- **Bar charts** (experience)
- **Pie charts** (education & location)
- **Statistical summaries** & interactive data points

---

## 🗂️ Project Structure

1. **Resume Upload**
   - Single PDF file upload
   - Text extraction
   - Store in CSV

2. **Basic Analysis**
   - Extract skills (keyword matching)
   - Calculate years of experience
   - Detect education level

3. **Simple Matching**
   - Compare to predefined skill requirements
   - Generate match score
   - Display results in table

---

## 🗄️ Data Storage

**CSV Structure:**

`resumes.csv`
- `resume_id`
- `extracted_text`
- `skills_found`
- `match_score`

---

## 🛠️ API Endpoints

| Endpoint                | Description                  |
|-------------------------|-----------------------------|
| `POST /api/upload`      | Upload resume               |
| `GET /api/results/{id}` | Get analysis results        |

---

## 🏗️ Step-by-Step Setup Guide

**Pre-requisites:**  
- Python  (preferably v11; _avoid v13 as it may lack some packages_)  
- Node.js (latest LTS recommended)

> _If you lack Python/Node.js, search "install Python 11" and "install Node.js" on Google and follow your OS-specific instructions._

---

### 1️⃣ Clone the Repository

```sh
git clone https://github.com/SyedHasanHussainShah/Resume-Screen.git
cd resume-screening-system-using-ml
```

---

### 2️⃣ Back-End Setup (FastAPI)

```sh
cd backend
```

**Create & activate a Python virtual environment:**

```sh
# Linux/macOS
python -m venv venv
source venv/bin/activate

# Windows PowerShell
python -m venv venv
venv\Scripts\activate
```

**Install requirements:**

```sh
pip install -r requirements.txt
```

**Start the API server:**

```sh
uvicorn resume-screener:app --reload
```

_If successful, you should see FastAPI starting (default port: **8000**). If you see a 404 error, let us know!_

**Test API:**  
Visit [http://127.0.0.1:8000](http://127.0.0.1:8000) in your browser.

---

### 3️⃣ Front-End Setup (React)

In a **new terminal**, navigate to the frontend folder:

```sh
cd resume-screening-system-using-ml-main\resume-screener
```

**Install dependencies:**

```sh
npm install
```

**Start the React dev server:**

```sh
npm run dev
```

_UI is typically available at:_  
[http://localhost:5173/](http://localhost:5173/)

---

### 4️⃣ Login Credentials

| Username | Password   |
|----------|------------|
| admin    | admin123   |

---

### 5️⃣ Verify Everything Works

- Open the frontend in your browser
- Upload a job description and one or more resumes
- Enjoy animated feedback: **match scores, dashboards, rankings, and more!**

---

> **Happy screening!** 🎉  
> _For issues, refer to the repo or raise a GitHub issue._
