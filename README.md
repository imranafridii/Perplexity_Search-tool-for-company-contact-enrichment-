# Lead Enrichment Automation with n8n & SerpApi

## 🚀 Overview
This project automates the process of finding LinkedIn profiles for a list of companies stored in Google Sheets. It eliminates manual research and ensures data consistency.

## 🛠️ Tech Stack
- **n8n:** Workflow Orchestration
- **SerpApi:** Google Search API for LinkedIn extraction
- **Google Sheets:** Data storage and source

## 📂 Workflow Nodes
1. **Read Node:** Fetches data from Google Sheets.
2. **Filter Node:** Logic gate to process only rows with an 'Empty' status.
3. **HTTP Request:** Connects to SerpApi for automated searching.
4. **Edit Fields:** Parses JSON data into clean LinkedIn URLs.
5. **Update Node:** Writes results back to Google Sheets and marks as 'Done'.

## 📖 How to Use
1. Import the `json` file into your n8n instance.
2. Configure your Google Sheets credentials.
3. Add your SerpApi Key in the HTTP Request node.
4. Execute the workflow.
