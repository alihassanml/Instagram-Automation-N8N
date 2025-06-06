# 📸 Instagram Automation with n8n & Apify
![workflow](./)

This workflow automatically:

1. Scrapes Instagram posts (latest & top performers)  
2. Identifies warm leads engaging with these posts  
3. Captures data like username, engagement, and last post URL  
4. Routes leads for manual review and outreach  
5. Connects with follow-up messaging and session tracking (AI/human handoff)  

Built using **n8n** + **Apify** + optional **PhantomBuster**, **OpenAI**, **MongoDB**, and automated publishing tools.

---

## 🚀 Features

- **Scheduled scraping**: trigger daily or on-demand  
- **Lead detection**: extract engaged users who are not yet followers  
- **Human-in-the-loop**: review & approve leads manually  
- **Personalized outreach**: generate messages via GPT-3.5  
- **Session tracking**: manage AI/human conversations  
- **Post repurposing (future)**: transform content for multiple platforms  
- **Reporting**: get summaries via email/Supabase/Google Sheets

---

## 🔧 Prerequisites

- Self-hosted or cloud-based **n8n** instance  
- **Apify** Instagram scraper or **PhantomBuster** account  
- Optional: MongoDB or Supabase for session/state tracking  
- OpenAI API key (for GPT messaging/content)  
- Meta Graph API credentials (for future automatic posting)

---

## 🧩 Flow Overview

1. **Trigger** – via schedule or webhook  
2. **Scrape Instagram** – fetch new/top post URLs  
3. **Extract leads** – scrape user info & filter warm leads  
4. **Manual review** – lead verification dashboard  
5. **Outreach** – send AI-generated personalized messages  
6. **Session management** – track conversation state  
7. **(Later)** Repurpose content – convert IG posts into blogs/images/etc.  
8. **Reporting** – send notifications and logs

---

## 🎯 Setup Steps

1. Clone the repo:  
   ```bash
   git clone https://github.com/alihassanml/Instagram-Automation-N8N.git
   cd Instagram-Automation-N8N
