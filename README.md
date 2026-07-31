# 🤖 AI Email Assistant with n8n

![n8n](https://img.shields.io/badge/n8n-Automation-EA4B71?style=for-the-badge&logo=n8n&logoColor=white)
![OpenRouter](https://img.shields.io/badge/OpenRouter-LLM-blue?style=for-the-badge)
![Gmail](https://img.shields.io/badge/Gmail-API-EA4335?style=for-the-badge&logo=gmail&logoColor=white)
![Google Sheets](https://img.shields.io/badge/Google%20Sheets-34A853?style=for-the-badge&logo=googlesheets&logoColor=white)
![Telegram](https://img.shields.io/badge/Telegram-Bot-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

An AI-powered email automation workflow built with **n8n** that intelligently analyzes incoming Gmail messages using an LLM through **OpenRouter**. The workflow classifies emails, detects sentiment, assigns priority, determines whether a reply is required, generates professional response drafts, logs activities, and notifies users for human review.

---

# 📖 Overview

## Problem

Managing email manually becomes increasingly difficult as inbox volume grows. Teams often spend valuable time reading, categorizing, prioritizing, and responding to repetitive messages.

Common challenges include:

- Slow response times
- Manual email classification
- Missed high-priority messages
- Inconsistent reply quality
- Limited visibility into email activity

## Solution

This workflow automates the email triage process using AI while keeping humans in control before sending replies.

The system automatically:

- Monitors incoming Gmail messages
- Extracts email details
- Uses AI to analyze message content
- Classifies category and priority
- Detects sentiment
- Determines if a reply is required
- Generates professional reply drafts
- Stores audit logs in Google Sheets
- Sends Telegram notifications for actionable emails

---

# ✨ Features

## 📥 Email Processing

- Monitor incoming Gmail messages
- Extract sender, subject, and message body
- Detect actionable emails
- Track email activity automatically

## 🤖 AI Analysis

- AI-generated summaries
- Automatic email categorization
- Priority detection (Low, Medium, High)
- Sentiment analysis
- Reply requirement detection
- Professional reply generation

## 📊 Workflow Automation

- Conditional routing based on priority
- Human-in-the-loop approval process
- Google Sheets audit logging
- Telegram notifications
- End-to-end workflow automation

---

# 🏗 Workflow Architecture

```text
                    Gmail Trigger
                          │
                          ▼
              Retrieve Email Details
                          │
                          ▼
                Prepare Email Data
                          │
                          ▼
               AI Email Analysis (LLM)
                          │
                          ▼
            Parse Structured AI Output
                          │
                          ▼
                Priority-Based Routing
                          │
             ┌────────────┴────────────┐
             ▼                         ▼
      Reply Required?              No Reply
             │                         │
      ┌──────┴──────┐                  │
      ▼             ▼                  ▼
Generate Reply   Save Log        Save Log
      │
      ▼
Google Sheets
      │
      ▼
Telegram Notification
      │
      ▼
 Human Review
```

---

# 📸 Workflow Screenshot

<p align="center">
  <img src="images/workflow.png" alt="Workflow" width="100%">
</p>

---

# 🛠 Tech Stack

## Workflow Automation

- n8n

## Artificial Intelligence

- OpenRouter
- Large Language Models (LLMs)

## APIs & Integrations

- Gmail API
- Google Sheets API
- Telegram Bot API

## Programming

- JavaScript

---

# 📂 Repository Structure

```text
AI-Email-Assistant-with-n8n/

├── README.md
├── AI Email Assistant.json
├── images/
│   └── workflow.png
└── LICENSE
```

---

# ⚙️ Setup Guide

## 1. Clone the Repository

```bash
git clone https://github.com/belioautomation/AI-Email-Assistant-with-n8n.git
```

---

## 2. Import the Workflow

Import the included workflow into your n8n instance.

```text
AI Email Assistant.json
```

---

## 3. Configure Credentials

Configure the following credentials inside n8n:

- Gmail OAuth2
- OpenRouter API
- Google Sheets OAuth2
- Telegram Bot

---

## 4. Update Configuration

Customize:

- Gmail labels (optional)
- AI prompts
- Google Sheets destination
- Telegram Chat ID

---

## 5. Activate Workflow

Once all credentials are configured, activate the workflow.

---

# 📊 Example Workflow

```text
Incoming Email
        │
        ▼
AI Analysis
        │
        ▼
Priority Classification
        │
        ▼
Reply Decision
        │
        ▼
Reply Draft
        │
        ▼
Google Sheets Log
        │
        ▼
Telegram Notification
```

---

# 📄 Example AI Output

```json
{
  "summary": "Customer is requesting a refund for a recent purchase.",
  "category": "Billing",
  "priority": "HIGH",
  "sentiment": "NEGATIVE",
  "requiresReply": true,
  "draftReply": "Thank you for reaching out. We're reviewing your request and will get back to you shortly."
}
```

---

# 💡 Business Value

This workflow helps organizations:

- Reduce manual email processing
- Improve response consistency
- Prioritize critical emails automatically
- Generate AI-assisted replies
- Maintain human approval before sending responses
- Create searchable audit logs
- Increase operational efficiency

---

# 🎯 Skills Demonstrated

- AI Workflow Automation
- n8n Development
- OpenRouter Integration
- Gmail API Integration
- Google Sheets Automation
- Telegram Bot Integration
- Prompt Engineering
- Structured AI Outputs
- Conditional Workflow Routing
- Human-in-the-Loop Automation
- Business Process Automation

---

# 🔮 Future Improvements

- Gmail draft creation
- Automatic approval rules
- Multi-user approval workflows
- CRM integration
- Slack / Microsoft Teams notifications
- AI confidence scoring
- Analytics dashboard
- Email categorization history

---

# 👨‍💻 Author

**Belio C. Sinangote**

BS Information Technology Student  
AI Automation Developer | n8n Workflow Builder

**GitHub:** https://github.com/belioautomation

**LinkedIn:** https://www.linkedin.com/in/belio-sinangote-180375402/

---

# 📄 License

This project is licensed under the **MIT License**.

---
