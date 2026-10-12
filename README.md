*Intuz — Your automation partner, one workflow at a time.*

<p align="center">
  <picture>
    <img alt="Banner Image" src="https://github.com/user-attachments/assets/210f97fc-0fce-404a-b647-7dfe1302cd37" />
  </picture>
</p>

[Intuz](https://www.intuz.com) helps organizations orchestrate AI, automation, and enterprise systems through scalable workflows. Our repository showcases proven implementations across healthcare, operations, customer support, document processing, sales, and back-office functions, enabling teams to accelerate automation initiatives without starting from scratch.

[N8N Creator](https://n8n.io/creators/intuz/) · [Generative AI Development](https://www.intuz.com/generative-ai-development/) · [Custom AI Development](https://www.intuz.com/ai/) · [For Custom Workflow Automation](https://www.intuz.com/get-started/)

# Personalized sales outreach from LinkedIn job signals with Apify & Google Gemini

> Community nodes are used in this workflow. This template can only be used on **self-hosted n8n instances**.
<img width="1021" height="479" alt="Overview_f6ae317cd5" src="https://github.com/user-attachments/assets/a61d708c-3ba4-4a4f-a222-fc733c558d7c" />

This n8n template from Intuz provides a complete and automated solution for identifying high-intent leads from LinkedIn job postings and automatically generating personalized outreach emails.

## Who’s this workflow for?

- B2B Sales Teams & SDRs
- Recruitment Agencies & Tech Recruiters
- Startup Founders
- Growth Marketing Teams

## How it works

1. **Scrape Hiring Signals:** The workflow starts by using an Apify scraper to find companies actively hiring for specific roles on LinkedIn (e.g., “ML Engineer”).

2. **Filter & Qualify Companies:** It automatically filters the results based on your criteria (e.g., company size, industry) to create a high-quality list of target accounts.

3. **Find Decision-Makers:** For each qualified company, it uses Apollo.io to find key decision-makers (VPs, Directors, etc.) and enrich their profiles with verified email addresses using the user’s Apollo API.

4. **Build a Lead List:** All the enriched lead data—contact name, title, email, company info—is systematically added to a Google Sheet.

5. **Generate AI-Powered Emails:** The workflow then feeds each lead’s data to a Google Gemini AI model, which drafts a unique, personalized cold email that references the specific job the company is hiring for.

6. **Complete the Outreach List:** Finally, the AI-generated subject line and email body are saved back into the Google Sheet, leaving you with a fully prepared, hyper-targeted outreach campaign.

## Setup Instructions

### 1. Apify Configuration

- Connect your Apify account in the **Run the LinkedIn Job Scraper** node.
- You’ll need an Apify scraper — we have used this scraper in the template.
- In the **Custom Body** field, paste the URL of your target LinkedIn Jobs search query.

### 2. Data Enrichment

- Connect your account API of data providers like Clay, Hunter, Apollo, etc. using HTTP Header Auth in the **Get Targeted Personnel** and **Email Finder** nodes.

### 3. Google Gemini AI

- Connect your Google Gemini (or PaLM) API account in the **Google Gemini Chat Model** node.

### 4. Google Sheets Setup

- Connect your Google Sheets account.
- Create a spreadsheet and update the Document ID and Sheet Name in the three Google Sheets nodes to match your own.

### 5. Activate Workflow

- Click **Execute workflow** to run the entire lead generation and email-writing process on demand.

## FAQ

**Is this template free to use?**
Yes. It's an open-source n8n workflow published by Intuz — copy the workflow JSON from this repo and import it into your own n8n instance at no cost.

**Do I need a paid n8n plan to run this?**
This template uses community nodes, so it only runs on **self-hosted n8n**. You'll need your own credentials for Apify, Apollo (or another enricher), Google Gemini, and Google Sheets.

**Does it send the emails automatically?**
No. It finds hiring companies on LinkedIn, enriches decision-makers, drafts Gemini-personalized emails that reference the open role, and writes them to Google Sheets for you to review and send.

## Related n8n templates from Intuz

- [Automate LinkedIn profile research & email outreach with Apify, Gemini & Sheets](https://github.com/Intuz-production/LinkedIn-Lead-Generation-Automation)
- [Automate lead gen & email outreach with Apify, Apollo.io, GPT-4 & Google Sheets](https://github.com/Intuz-production/AI-Lead-Generation-Automation)
- [Automate cold outreach with email personalization using Gemini and Google Sheets](https://github.com/Intuz-production/Personalized-Sales-Outreach-Automation-with-AI)

[See all of Intuz's free n8n templates](https://www.intuz.com/n8n-workflow-automation-templates/)

## Connect with us

Intuz is a USA-based AI & workflow automation company with 16+ years of experience building custom AI-enabled workflow automations for SMBs and Enterprises, specializing in agentic AI, LLM integrations, and CRM/ERP sync across Healthcare, FinTech, eCommerce, Manufacturing, and Real Estate.

* **Website:** [https://www.intuz.com](https://www.intuz.com)
* **Email:** [getstarted@intuz.com](mailto:getstarted@intuz.com)
* **LinkedIn:** https://www.linkedin.com/company/intuz/
* **Get Started:** https://n8n.partnerlinks.io/intuz

## For Custom Workflow Automation

[Click here - Get Started](https://www.intuz.com/get-started/)
