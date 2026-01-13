# Upwork Automation Agent for Morgan 🤖

## 📌 Project Overview
This project is an automated lead generation workflow built in **n8n**. It scrapes Upwork job listings via **Apify**, analyzes them using **AI (Gemini/OpenAI)** to score their relevance for an Automation Engineer (Morgan), and saves qualified leads into **Airtable**.

## 🚀 Features
- **Smart Scoring:** Uses AI to score jobs (1-10) based on specific skills (n8n, Make, API integration).
- **Rate Limit Protection:** Implements a `Loop` and `Wait` mechanism to prevent API 429 errors.
- **Data Integrity:** Strict JSON Parsing ensures no job details (Title, URL) are lost during AI processing.
- **Cost Efficient:** Pre-filters "Entry Level" jobs to save on AI token costs.

## 🛠️ Setup Instructions
1. **Import Workflow:** Download `Upwork-Final.json` from this repo and import it into your n8n instance.
2. **Configure Credentials:**
   - **Apify:** Add your API Token.
   - **Google Gemini (or OpenAI):** Add your API Key.
   - **Airtable:** Connect your account and select your Base/Table.
3. **Run:** Execute the workflow manually or wait for the scheduled trigger (every 8 hours).

## 📂 Deliverables
- `Upwork-Final.json`: The complete workflow file.
- `Project-Report.pdf`: Details of issues fixed and sample data.
