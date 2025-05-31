🤖 AI-Powered Instagram Workflow with n8n
Automated Content Creation + Direct Publishing from Google Sheets


✨ Overview
This n8n workflow automates your entire Instagram content execution pipeline — from content ideas in a Google Sheet to AI-generated posts published directly on Instagram.

It leverages:

🧠 Google Gemini (Vertex AI) for content concepts, image prompts, and captions

🎨 Replicate (Flux model) for generating unique visual content

📄 Google Sheets as the content planning interface

📲 Facebook Graph API to publish directly to Instagram Business

🚀 Features
✅ Automatically fetches pending post ideas from Google Sheets
✅ Generates platform-specific concepts, prompts, and captions using AI
✅ Creates visuals via Replicate's Flux model
✅ Publishes directly to Instagram Business account
✅ Updates Google Sheet to avoid duplicate posting
✅ Fully customizable in n8n

📁 Folder Structure
bash
Copy
Edit
📦 instagram-ai-workflow/
 ┣ 📄 README.md
 ┣ 📄 workflow.json            # ✅ Import this into n8n
 ┗ 📄 preview.png              # 🖼️ Visual flowchart of the workflow
🧰 Prerequisites
Before importing the workflow, ensure you have:

A running n8n instance (Cloud or Self-hosted)

A Google Sheet with columns: Topic, Audience, Voice, Platform, Status (pending = 0, completed = 1)

Google Sheets API credentials in n8n (OAuth2)

Google Vertex AI credentials (for Gemini)

A Replicate account with API token (Header Auth)

A Facebook Developer account and:

Instagram Business Account linked to a Facebook Page

App permissions: instagram_basic, instagram_content_publish, pages_read_engagement, pages_show_list

Facebook Graph API OAuth2 credentials in n8n

🔧 Setup Instructions
Clone this repo or download the workflow.json

Go to your n8n instance → Import Workflow

Connect your credentials to the following nodes:

Google Sheets

Google Gemini (Vertex AI)

Replicate (Header Auth)

Facebook Graph API (OAuth2)

Update:

Your Spreadsheet ID & Sheet Name

Your Instagram Account ID in publishing steps

Adjust the Schedule Trigger to run every hour, 4 hours, etc.

Add your content ideas to the Google Sheet with status 0

Activate the workflow. Done! 🎉

🧪 Demo Use Case
Plan 30 days of Instagram content in Sheets → Let this workflow handle everything else 💼

📬 Get in Touch
If you need help customizing this or want to extend to LinkedIn, Facebook, or X (Twitter), feel free to open an issue or drop me a message.

📜 License
MIT License – free to use, share, and modify.

