# LinkedIn Profile Finder Automation

This project automatically finds **real LinkedIn profile links** using simple input from Google Sheets.

Instead of manually searching LinkedIn or Google, you just enter a job role and location (for example:  
`machine learning engineer india`) in a Google Sheet, and the system does the rest.

---

## How It Works

1. You add a job role and location in a Google Sheet  
2. The automation reads the input  
3. An AI model converts it into a Google search query  
4. The search is restricted to **only LinkedIn personal profiles**  
5. Matching LinkedIn profile links are collected  
6. Results are saved back into a Google Sheet automatically  

No chat input or manual searching is needed.

---

## Input Format (Google Sheet)

Sheet name: `Input`

Column name:
chatInput

makefile
Copy code

Example:
machine learning engineer india
data scientist berlin
product manager san francisco

yaml
Copy code

Each row is treated as a new search request.

---

## Output

The output Google Sheet contains:
- Profile title
- LinkedIn profile link
- Short description/snippet

Only personal LinkedIn profiles are included.  
Company pages, job posts, and other links are excluded.

---
🔍 Real-world Use Case
B2B Lead Generation / Sales Prospecting
Perfect for:

Sales teams

Recruiters

Startup founders

Marketing agencies

Freelancers doing outreach

🎯 Practical Scenarios
🔹 Recruiters
“Find 50 Java Developers in Mumbai without opening LinkedIn”

🔹 SaaS founders
“Build a list of CTOs to pitch my product”

🔹 Marketing agencies
“Collect LinkedIn profiles for cold DM campaigns”

🔹 Freelancers
“Get decision-makers for proposal outreach”

---

## Tech Stack

- n8n (workflow automation)
- Google Sheets
- OpenAI / LLM
- Google Search API (Serper)

---

## Notes

- The workflow is low-code and easy to customize  
- Can be extended with auto-triggers, duplicate removal, or status tracking  
- Designed to save time and reduce manual effort  

---

## Author

Built as a practical AI automation project to streamline LinkedIn profile discovery

