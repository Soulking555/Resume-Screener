# AI Resume Screening System

An intelligent web-based Resume Screening System that automates
candidate evaluation using Natural Language Processing (NLP) and
similarity matching techniques.

------------------------------------------------------------------------

## Project Description

The AI Resume Screening System is a frontend-based application that
compares candidate resumes with a given job description and ranks
candidates based on relevance, skills, experience, and education.

It simulates the working of an Applicant Tracking System (ATS) using
client-side JavaScript and NLP techniques.

------------------------------------------------------------------------

## Features

-   Paste Job Description
-   Add multiple resumes
-   Upload PDF (demo mode)
-   Automatic:
    -   Skill extraction
    -   Experience detection
    -   Education identification
    -   Cosine similarity calculation
-   Weighted scoring algorithm
-   Candidate ranking
-   Recommendation classification
-   Skill match visualization
-   Clean responsive UI

------------------------------------------------------------------------

## How It Works

### Step 1 -- Text Preprocessing

-   Convert text to lowercase
-   Remove stopwords
-   Tokenize text

### Step 2 -- Keyword Extraction

-   Predefined technical skills list
-   Match keywords from job description and resume

### Step 3 -- Feature Extraction

-   Education level detection (PhD, Master, Bachelor, etc.)
-   Experience extraction (years/months detection using RegEx)

### Step 4 -- Similarity Matching

-   Cosine similarity between:
    -   Job keywords and resume keywords
    -   Overall job and resume text

### Step 5 -- Weighted Scoring

Final Score Formula:

Final Score = (0.4 × Skill Score) + (0.25 × Keyword Match) + (0.15 ×
Overall Similarity) + (0.15 × Experience Score) + (0.05 × Education
Score)

### Step 6 -- Ranking

Candidates are sorted in descending order and classified as:

-   Highly Recommended
-   Recommended
-   Maybe
-   Not Recommended

------------------------------------------------------------------------

## Technologies Used

### Frontend

-   React 18 (CDN UMD)
-   ReactDOM
-   Babel Standalone
-   Tailwind CSS

### JavaScript APIs

-   FileReader API
-   Regular Expressions
-   Array & String Methods

### Algorithms

-   Cosine Similarity
-   Tokenization
-   Stopword Removal
-   Rule-based NLP

------------------------------------------------------------------------

## Project Structure

resume_screener.html

Single-page architecture: - React Component: ResumeScreener - NLP
Utility Functions - Scoring Engine - Modal Management - UI Rendering

------------------------------------------------------------------------

## Installation & Usage

### Direct Run

1.  Download the HTML file.
2.  Open in any modern browser (Chrome recommended).
3.  Click "Load Sample Data" or manually add data.
4.  Click "Screen Resumes".

No server required.

------------------------------------------------------------------------

## Future Improvements

-   Backend integration (Flask / Node.js)
-   Real PDF parsing (pdf.js)
-   TF-IDF Vectorization
-   Machine Learning Model (Naive Bayes / Logistic Regression)
-   Resume Database
-   Recruiter Dashboard
-   Authentication
-   Cloud Deployment

------------------------------------------------------------------------

## Conclusion

This AI Resume Screening System provides a simplified but functional
implementation of automated candidate ranking using rule-based NLP and
similarity matching. It can serve as a foundation for building a
full-scale ATS powered by machine learning.
