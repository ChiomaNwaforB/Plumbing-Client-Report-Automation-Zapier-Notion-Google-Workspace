# Plumbing-Client-Report-Automation-Zapier-Notion-Google-Workspace
Automated client report generation for a plumbing business using Zapier, Notion, Google Docs, Google Drive, and Gmail. The workflow generates personalized PDFs, emails them to clients and uses status-based controls to prevent premature execution and duplicate processing.

# Project Overview
This project automates the generation and delivery of plumbing service reports by integrating Notion, Google Docs, Google Drive, Gmail, and Zapier.

When a client's record is updated and marked as Ready, the workflow automatically generates a customized report using a Google Docs template, exports it as a PDF, emails it to the client and updates the client record to Sent.

The automation eliminates repetitive manual work while ensuring reports are only processed when all required client information has been completed.

# Business Problem
The plumbing company stored client information in a Notion database but relied on a manual process to:

Create individual client reports.
Replace client details in a report template.
Convert the report into a PDF.
Send the report via email.
Track whether a report had already been sent.

Using a simple New Database Item trigger would also introduce another problem: the workflow could execute immediately after a client record was created, even before all required information had been entered, resulting in incomplete reports and unnecessary emails.

# Challenges Identified
Client records are often created before all details are available.
Premature automation could generate incomplete reports.
Duplicate emails could be sent if records were updated multiple times.
Manual document generation consumed valuable administrative time.
The reporting process lacked a reliable completion tracking mechanism.

# Solution
Designed a workflow that mirrors the company's real business process rather than simply automating database creation events.

Instead of triggering whenever a new record was added, the automation monitors updates to the database and only proceeds when the record's Status changes to Ready.

Once approved, the workflow:
Retrieves client information from Notion.
Generates a personalized Google Doc from a predefined template.
Exports the document as a PDF.
Sends the PDF to the client via Gmail.
Updates the client's status to Sent, preventing duplicate processing.

# Key Features
- Automated client report generation from Notion data.
- Dynamic population of Google Docs templates.
- Automatic PDF export.
- Automated email delivery with PDF attachment.
- Status-based workflow control using Filter by Zapier.
- Trigger based on Updated Properties in Data Source Item instead of record creation.
- Automatic status update to Sent after successful email delivery.
- Duplicate email prevention.
- Fully scalable workflow requiring no manual intervention after setup.

# Tech Stack
Zapier – Workflow automation and orchestration
Notion – Client database
Google Docs – Dynamic document generation
Google Drive – Document export
Gmail – Automated email delivery

# Business Impact
Reduced manual document preparation and emailing.
Eliminated repetitive administrative tasks.
Prevented incomplete reports from being generated.
Reduced the risk of duplicate client communications.
Improved workflow reliability through status-based automation.
Created a scalable, standardized process for generating and delivering client reports.
Improved operational efficiency by allowing staff to focus on customer service rather than repetitive document management.

# Workflow


# Skills Demonstrated
- Workflow Automation
- Zapier
- Business Process Analysis
- No-Code Automation
- Google Workspace Integration
- Notion Automation
- Conditional Logic
- Process Optimization
- Systems Thinking
- Workflow Design
- Business Operations Automation
