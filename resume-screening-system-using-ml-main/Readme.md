# Resume Screening Application

A modern resume screening application that helps recruiters analyze and compare candidates efficiently.

## Project Overview

A React-based application that streamlines the resume screening process by providing:
- PDF document uploads for job descriptions and resumes
- Automated skill matching and scoring
- Visual analytics and demographics
- Candidate ranking system
- Shortlisting and report generation

## Features

### Document Upload
- Drag-and-drop interface for both job descriptions and resumes
- Multi-file upload support for resumes
- Progress tracking for file uploads
- PDF format validation
- Visual feedback during upload process

### Analysis & Matching
- Automated skill extraction and matching
- Match score calculation based on required skills
- Experience and education level detection
- Location-based grouping

### Results & Analytics
1. **Demographics Dashboard**
   - Experience distribution chart
   - Education level breakdown
   - Geographic distribution
   - Key statistics:
     - Total candidates
     - Average experience
     - Average match score
     - Most common location

2. **Candidate Rankings**
   - Sorted by match score
   - Medal system for top 3 candidates
   - Detailed candidate cards showing:
     - Match percentage
     - Found skills
     - Missing required skills
     - Experience details
     - Education information
     - Location

3. **Shortlisting Features**
   - Candidate selection system
   - PDF report generation for shortlisted candidates
   - Downloadable summary of selected candidates

## Tech Stack

### Frontend
- React.js
- Tailwind CSS for styling
- Chart.js for data visualization
- PDF-lib for report generation

### UI Components
- Drag and drop file upload
- Progress bars
- Interactive charts
- Responsive design
- Modal dialogs

### Data Visualization
- Bar charts for experience distribution
- Pie charts for education and location
- Statistical summaries
- Interactive data points

## Project Structure

1. **Resume Upload**
   - Single PDF file upload
   - Text extraction
   - Store in CSV

2. **Basic Analysis**
   - Extract skills using keyword matching
   - Calculate years of experience (if mentioned)
   - Basic education level detection

3. **Simple Matching**
   - Compare against predefined skill requirements
   - Generate basic matching score
   - Show results in simple table

## Data Storage

Simple CSV structure:

1. **resumes.csv**
   - resume_id
   - extracted_text
   - skills_found
   - match_score

## API Endpoints
- POST /api/upload - Upload resume
- GET /api/results/{resume_id} - Get analysis results


## Step-by-Step Setup Guide

These steps assume you're on a system with Python and Node.js (or Yarn) installed.

if not go to google serach python and install python version 11 not install 13 bcz it may lack some packages then for 
node.js install in google search node.js and download it according to your coressponding device

1. Clone the repository or Download the repo 
git clone https://github.com/SyedHasanHussainShah/Resume-Screen.git
cd resume-screening-system-using-ml

## Set up the Backend (FastAPI)

Navigate to the backend folder:

cd backend


## Create and activate a Python virtual environment:

python -m venv venv
source venv/bin/activate   # Linux/macOS
venv\Scripts\activate      # Windows PowerShell


## Install required packages:

pip install -r requirements.txt


## Start the API server:

uvicorn resume-screener:app --reload

If its work successfully then show application strat Something like message 
if show 404 error then tell us 

You should see FastAPI starting (default port should be 8000).

After running

Open your browser at: http://127.0.0.1:8000

this site can open 

## Set up the Frontend (React)

Open a new commad prompt in vs code, and navigate to the frontend folder (usually resume-screener or similar):

cd resume-screening-system-using-ml-main\resume-screener

## Install dependencies:

npm install  


## Start the React dev server:

npm run dev  


The UI should now be available (often on localhost:3000).

Go to that link

Local:   http://localhost:5173/

## Username and Password 

Username: admin
Password: admin123

## Verify Everything Works Together

Open the frontend in your browser.

Upload a job description and resume(s).

The interface should provide animated feedback: match scores, dashboards, rankings, etc.
