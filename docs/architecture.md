# System Architecture

This automation system orchestrates job search and application workflows using **n8n** as the central automation engine.

## Main Components

1. **Telegram Bot Interface**

   * User interaction layer
   * Receives commands and job search requests

2. **n8n Workflow Engine**

   * Handles orchestration
   * Processes automation logic
   * Integrates APIs

3. **Job Data Sources**

   * Apify scraping actors
   * External job platforms

4. **AI Processing Layer**

   * Generates personalized cover letters
   * Processes job descriptions
   * Uses LLM via OpenRouter

5. **Data Storage**

   * Google Sheets for user profiles
   * Job application tracking

6. **Automation Layer**

   * Browser automation
   * Job form submission
   * Application tracking

## Workflow Overview

User → Telegram Bot → n8n Workflow →
Job Search API → AI Cover Letter →
Automated Application → Status Update → Telegram Notification
