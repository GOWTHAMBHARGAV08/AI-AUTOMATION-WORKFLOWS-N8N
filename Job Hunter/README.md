# Job Hunter

An n8n workflow designed to automate job hunting by analyzing job listings against a resume, scoring them, and drafting personalized outreach emails or improvement suggestions.

## 🚀 Features

- **Automated Resume Parsing**: Extracts key details from a PDF resume.
- **Job Matching**: Compares job listings (fetched via JSearch API) against your skills and salary expectations.
- **Smart Scoring**: Uses OpenAI to score job suitability on a 0-10 scale.
- **Email Drafting**: Automatically drafts outreach emails for high-match jobs.
- **Skill Gap Analysis**: Identifies missing skills for potential opportunities.

## 🛠️ How It Works

1. **Trigger**: Starts on a schedule.
2. **Fetch Resume**: Downloads and extracts text from your resume (PDF).
3. **Search Jobs**: Queries the JSearch API for relevant job listings (e.g., "Software Engineer").
4. **Analyze**:
   - Normalizes salary data.
   - Compares candidate skills vs. job requirements.
   - Scores the match.
5. **Action**:
   - **High Match (7+)**: Generates a personalized email draft.
   - **Gap Analysis**: Lists areas for improvement if the match is close but missing key skills.
6. **Notification**: Sends a summary email with job cards and drafts.

## ⚙️ Setup

1. **Import Workflow**: Load `Job Hunter.json` into n8n.
2. **Configure Credentials**:
   - **Gmail**: For sending notifications.
   - **Google Drive**: To access your resume.
   - **OpenAI**: For analysis and drafting.
   - **JSearch API**: To fetch job listings.
3. **Update Resume Link**: Ensure the Google Drive node points to your current resume.
4. **Adjust Search Query**: Modify the `Call JSearch API` node to target your desired role and location.

## 📋 Requirements

- n8n (Self-hosted or Cloud)
- OpenAI API Key
- JSearch API Key
- Google Cloud Credentials (Drive & Gmail)
