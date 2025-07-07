# SAP B1 Customer Support Automation Workflow 🚀

### Demo Video
[<img src="https://via.placeholder.com/600x300.png?text=Watch+SAP+B1+Automation+Demo" alt="SAP B1 Workflow Demo" />](https://github.com/zeineb61romthana/SAP-B1-Customer-Support-Automation-Workflow/blob/main/ezgif.com-video-to-gif-converter.gif)

Welcome to the **SAP B1 Customer Support Automation Workflow**, a powerful n8n-based solution that streamlines customer support for SAP Business One (SAP B1). This project automates the processing of customer emails, integrates with SAP B1’s OData API, generates reports, and manages support tickets, saving time and reducing manual effort.

## 🌟 Project Overview

This workflow automates customer support tasks by:
- Monitoring Gmail for customer requests (e.g., invoices, orders).
- Using AI to classify emails and extract key details.
- Interacting with SAP B1 to retrieve or create documents.
- Generating professional responses or support tickets when issues arise.
- Logging tickets in Google Sheets for easy tracking.

Built with [n8n](https://n8n.io/), this project showcases the power of low-code automation, AI, and ERP integration to enhance business efficiency.

## ✨ Key Features

- **📧 Smart Email Processing**: Filters and classifies incoming Gmail requests using AI (Mistral Cloud) to identify invoice or order requests.
- **🔄 Seamless SAP B1 Integration**: Authenticates with SAP B1 Service Layer, retrieves customer data, orders, and invoices, and creates new invoices as needed.
- **🤝 Accurate Customer Matching**: Matches customers by email, ensuring precise identification using SAP B1’s Business Partners data.
- **🕒 Session Management**: Handles SAP B1 session timeouts with automatic refresh for uninterrupted connectivity.
- **📄 Dynamic Report Generation**: Simulates Crystal Reports to produce PDF invoices or order confirmations.
- **🛠️ Robust Error Handling**: Detects failures, creates support tickets, and notifies customers with professional, empathetic emails.
- **📊 Ticket Tracking**: Logs support tickets in Google Sheets for streamlined follow-up.

## 🛠️ Workflow Structure

The workflow, defined in `My_workflow_7.json`, consists of n8n nodes that:
1. Trigger on new Gmail emails with keywords like "invoice" or "order."
2. Use AI to classify requests and extract details (e.g., order numbers).
3. Authenticate with SAP B1 and manage session validity.
4. Match customers against SAP B1 Business Partners by email.
5. Retrieve specific or latest orders/invoices or create new invoices.
6. Generate PDF reports and send professional email responses via Gmail.
7. Handle failures by creating tickets in Google Sheets and notifying customers.


## 📋 Prerequisites

To run this workflow, you’ll need:
- **n8n**: A self-hosted or cloud instance of n8n.
- **SAP B1 Service Layer**: Access to an SAP B1 instance with OData API (e.g., `https://<your-server>:50000/b1s/v1`).
- **Gmail Account**: OAuth2 credentials for Gmail to monitor and send emails.
- **Google Sheets**: OAuth2 credentials for storing support tickets.
- **Mistral Cloud**: API credentials for AI-powered email classification and response generation.
- **Git**: For cloning and managing the repository.
- **Node.js**: For executing custom code within n8n nodes.

## 🚀 Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/zeineb61romthana/SAP-B1-Customer-Support-Automation-Workflow.git
   cd SAP-B1-Customer-Support-Automation-Workflow
