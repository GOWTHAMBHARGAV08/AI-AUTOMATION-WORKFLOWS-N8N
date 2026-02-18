# n8n-social-media-auto-posting
An automated system for posting images and videos to multiple social media platforms — Instagram, LinkedIn, Pinterest, and X (Twitter) — using workflow automation, scheduling, and AI-generated content.

This project reduces manual posting effort and ensures consistent, scheduled content delivery across platforms.

🚀 Features

✅ Auto-post images and videos

⏰ Scheduled publishing (time-based automation)

📱 Supported platforms:

Instagram

LinkedIn

Pinterest

X (Twitter)

🤖 AI-generated titles & captions

🖼️ Image processing & metadata handling

🎥 Video posting with thumbnails

🔀 Platform-based routing logic

🧩 Easy to extend for additional platforms

🛠️ Tech Stack

n8n – Workflow automation

AI Agents (LLMs) – Caption & title generation

Airtable / Google Sheets – Content source

Webhooks & APIs – Platform integrations

JSON Workflows – Import/export ready

🧠 How It Works

Content (image/video, title, description) is stored in Airtable or Sheets.

The workflow:

Fetches content

Enhances copy using AI agents

Processes images or videos

Routes content based on the target platform (Instagram, LinkedIn, Pinterest, X)

Posts are published automatically at scheduled times.

The workflow runs continuously based on your defined schedule.

📁 Repository Structure
.
├── workflows/
│   └── auto-post-images-videos.json
├── docs/
│   └── workflow-overview.md
├── README.md

⚙️ Setup Instructions

Clone the repository:

git clone https://github.com/your-username/social-media-auto-posting.git


Open n8n

Import the workflow JSON file.

Configure:

Platform APIs (Instagram, LinkedIn, Pinterest, X)

Webhooks

Data source

Schedule timings

Activate the workflow 🚀

🎯 Use Cases

Personal brand automation

Startup & agency social media management

Scheduled marketing campaigns

AI-driven content distribution

📌 Roadmap

Carousel posting (Instagram & LinkedIn)

Platform-specific caption tuning

Error handling & retries

Analytics & performance tracking

Human approval step (optional)

📄 License

MIT License
Free to use, modify, and extend.
