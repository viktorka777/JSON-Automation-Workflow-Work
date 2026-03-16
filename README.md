![n8n](https://img.shields.io/badge/automation-n8n-orange)
![AI](https://img.shields.io/badge/AI-LLM-blue)
![Telegram](https://img.shields.io/badge/bot-Telegram-blue)
![Automation](https://img.shields.io/badge/workflow-automation-green)
![License](https://img.shields.io/badge/license-MIT-lightgrey)
📄 # n8n Job Search & Auto-Apply Workflow

This repository contains an advanced automation workflow built with n8n that automates the job search and application process using AI, APIs, and messaging integrations.

The workflow is designed to function as a Telegram-based job assistant, allowing users to search for jobs, generate personalized cover letters, and automatically apply to positions.

⚙️ Key Features

Telegram Bot Interface
Uses Telegram as the main user interaction channel.

Automated Job Search
Integrates with job scraping tools via Apify to retrieve job listings.

User Profile Management
Stores and retrieves user information using Google Sheets.

AI-Generated Cover Letters
Generates personalized cover letters using LLM models through OpenRouter.

Automated Job Applications
Uses automated browser actions (via Apify/Puppeteer actors) to fill and submit job application forms.

Parallel Job Search Execution
Runs job searches concurrently to improve performance.

Status Tracking
Updates job application status in Google Sheets.

🧠 Workflow Architecture

The workflow includes 58 automation nodes and consists of several logical modules:

1️⃣ Telegram Trigger

Receives user commands and button interactions.

2️⃣ Request Processing

Determines whether the user initiated:

a new job search

an application action

3️⃣ Job Search Engine

Fetches job listings using Apify actors and processes the results.

4️⃣ AI Cover Letter Generation

An AI agent generates a customized cover letter based on:

user profile

job description

5️⃣ Automated Application

Submits the application automatically via browser automation.

6️⃣ Feedback & Notifications

Sends confirmation and updates back to the user via Telegram.

🛠 Technologies Used

n8n

Telegram

Apify

Google Sheets

OpenRouter

LangChain nodes for AI orchestration

JSON workflow configuration


Disclaimer

This project is intended for educational and demonstration purposes only.

Users are responsible for complying with the terms of service of any platforms
integrated with this workflow.
