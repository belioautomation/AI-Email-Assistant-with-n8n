# 🤖 AI Email Assistant

![n8n](https://img.shields.io/badge/n8n-Automation-EA4B71?style=for-the-badge&logo=n8n&logoColor=white)
![OpenRouter](https://img.shields.io/badge/OpenRouter-AI-6C63FF?style=for-the-badge)
![Gmail](https://img.shields.io/badge/Gmail-API-D14836?style=for-the-badge&logo=gmail&logoColor=white)
![Google Sheets](https://img.shields.io/badge/Google%20Sheets-34A853?style=for-the-badge&logo=googlesheets&logoColor=white)
![Telegram](https://img.shields.io/badge/Telegram-Bot-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

An AI-powered email automation workflow built with **n8n**, **OpenRouter**, **Gmail**, **Google Sheets**, and **Telegram**. The workflow intelligently analyzes incoming emails, classifies them by category and priority, detects sentiment, determines whether a reply is required, generates professional response suggestions, and routes emails through a **Human-in-the-Loop (HITL)** approval process before any action is taken.

---

# 📖 Overview

## Problem

Managing large volumes of email manually is time-consuming and often leads to delayed responses, inconsistent communication, and missed high-priority messages. Traditional automation can also introduce risks when AI sends replies without human oversight.

## Solution

The AI Email Assistant combines AI-powered email analysis with a **Human-in-the-Loop (HITL)** workflow. Instead of automatically replying, the system generates structured insights and professional reply suggestions, allowing users to review and approve responses before they are sent.

This approach improves productivity while maintaining accuracy, accountability, and control over customer communications.

---

# ✨ Features

## 📥 Email Processing

- Monitor incoming Gmail messages automatically
- Retrieve sender, subject, and email content
- Standardize email data for AI processing

## 🤖 AI Analysis

- Generate concise email summaries
- Categorize emails automatically
- Detect sentiment
- Assign priority levels
- Determine if a reply is required
- Generate professional reply suggestions

## 👨‍💼 Human-in-the-Loop Review

- Store AI-generated replies for manual approval
- Prevent fully automated outbound emails
- Support safe AI-assisted communication

## 📊 Activity Tracking

- Log processed emails to Google Sheets
- Maintain an audit trail
- Track pending replies

## 📲 Notifications

- Send Telegram notifications for actionable emails
- Alert reviewers when human approval is required

---

# 🏗 Workflow Architecture

```
              Gmail Trigger
                    │
                    ▼
          Retrieve Email Details
                    │
                    ▼
            Prepare Email Data
                    │
                    ▼
          AI Email Analysis
                    │
                    ▼
      Parse Structured AI Output
                    │
                    ▼
           Route by Priority
                    │
                    ▼
        Reply Required Decision
           │                 │
           │ Yes             │ No
           ▼                 ▼
 Store Suggested Reply    Log Activity
           │                 │
           ▼                 ▼
 Log Email Activity      End Workflow
           │
           ▼
 Telegram Notification
```

---

# 📸 Workflow Screenshot

The image below shows the complete AI Email Assistant workflow implemented in **n8n**, including AI analysis, conditional routing, Google Sheets logging, and Telegram notifications.

<p align="center">
  <img src="images/workflow.png" alt="AI Email Assistant Workflow" width="100%">
</p>

---

# 🎥 Demo Video

Watch the complete workflow demonstration below.

📹 **Demo Video**

https://github.com/user-attachments/assets/YOUR_VIDEO_LINK

---

# 🛠 Tech Stack

## Workflow Automation

- n8n

## Artificial Intelligence

- OpenRouter
- Large Language Models (LLMs)
- Prompt Engineering
- Structured AI Outputs

## Google Workspace

- Gmail API
- Google Sheets API

## Notifications

- Telegram Bot API

## Programming

- JavaScript

---

# 📂 Repository Structure

```text
AI-Email-Assistant-with-n8n/

├── README.md
├── workflow/
│   └── AI Email Assistant.json
├── images/
│   └── workflow.png
├── LICENSE
└── demo.mp4
```

---

# ⚙️ Setup Guide

## 1. Clone Repository

```bash
git clone https://github.com/belioautomation/AI-Email-Assistant-with-n8n.git
```

## 2. Import Workflow

Import the workflow JSON into your n8n instance.

```
AI Email Assistant.json
```

## 3. Configure Credentials

Configure the following credentials inside n8n:

- Gmail OAuth2
- OpenRouter API
- Google Sheets OAuth2
- Telegram Bot API

## 4. Update Configuration

Modify the following based on your environment:

- Gmail inbox
- Google Sheets IDs
- Telegram Chat ID
- AI prompts
- OpenRouter model

## 5. Activate Workflow

Once credentials are configured, activate the workflow.

---

# 🧠 Example AI Output

```json
{
  "summary": "Customer requests a refund due to a billing issue.",
  "category": "Billing",
  "priority": "HIGH",
  "sentiment": "Negative",
  "requiresReply": true,
  "draftReply": "Thank you for contacting us. We have received your request and will review your refund as soon as possible."
}
```

---

# 📊 Google Sheets Structure

## Email Activity Log

| Timestamp | Sender | Subject | Category | Priority | Sentiment | Status |
|-----------|---------|----------|----------|----------|-----------|--------|

## Pending Reply Queue

| Timestamp | Sender | Subject | Suggested Reply | Priority | Status |
|-----------|---------|----------|----------------|----------|--------|

---

# 💼 Business Value

This workflow helps organizations:

- Reduce manual email processing
- Improve response consistency
- Prioritize urgent emails automatically
- Assist teams with AI-generated replies
- Maintain human oversight
- Keep a searchable audit history
- Increase operational efficiency

---

# 💡 Skills Demonstrated

- AI Workflow Automation
- Human-in-the-Loop Systems
- Prompt Engineering
- OpenRouter Integration
- Gmail API Integration
- Google Workspace Automation
- Telegram Bot Integration
- JavaScript Data Transformation
- Structured AI Outputs
- Enterprise Workflow Design

---

# 🚀 Future Improvements

- Gmail Draft creation
- Automatic approval rules
- Multi-user review system
- CRM integration
- Slack & Microsoft Teams support
- AI confidence scoring
- Analytics dashboard
- Email thread memory
- Multi-language support

---

# 👨‍💻 Author

**Belio C. Sinangote**

BS Information Technology Student  
AI Automation Developer | n8n Workflow Builder

GitHub: https://github.com/belioautomation

LinkedIn: https://www.linkedin.com/in/belio-sinangote-180375402/

---

# 📄 License

This project is licensed under the MIT License.

---
