## 💻 Computer Company Sales Bot
An automated AI-driven sales assistant built with n8n. This bot handles customer inquiries based on live inventory data and automates the post-purchase notification process.
## 🚀 How it Works

   1. Customer Inquiry: The bot receives a message via the chat interface.
   2. Data Retrieval: It queries a Google Sheet (inventory/knowledge base) to provide accurate answers about computer specs, pricing, and availability.
   3. AI Processing: An OpenAI-powered AI Agent processes the customer's intent and provides a natural, helpful response.
   4. Sales Notification: Once a purchase or high-intent lead is identified, the bot automatically sends an email via Gmail to the company owner with the customer's details.
   5. Version Control: Every time the workflow runs, it automatically backs itself up to this GitHub repository.

<img width="1440" height="900" alt="Screenshot 2026-05-10 at 11 36 16 PM" src="https://github.com/user-attachments/assets/a78138ee-d72f-4f5e-8654-69b7b72d1e2a" />


## 🛠️ Tech Stack

* Automation: n8n
* AI Engine: OpenAI (GPT-4 / GPT-3.5)
* Database: Google Sheets
* Communication: Gmail API
* Version Control: GitHub API

## 📂 Project Structure

* backup/: Contains the .json exports of the n8n workflows.
* README.md: Project documentation.

## ⚙️ Setup Instructions

   1. Import Workflow: Import the .json file from this repo into your n8n instance.
   2. Credentials: Set up the following credentials in n8n:
   * OpenAI API Key
      * Google Sheets OAuth2
      * Gmail OAuth2
      * GitHub Personal Access Token (for automated backups)
   3. Google Sheets: Ensure your sheet has columns for Item Name, Specs, Price, and Stock.
   4. Deployment: Toggle the workflow to Active.

