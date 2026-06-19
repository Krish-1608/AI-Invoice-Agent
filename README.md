#AI-Invoice-Agent

## Overview

AI Document Processing Agent is an intelligent workflow automation system designed for accounting and finance teams. The system automatically processes invoice emails, extracts key information from PDF invoices using AI, stores records in Airtable, sends team notifications, schedules payment reminders, and tracks invoice payment status.

## Problem

Accounting teams often spend significant time manually:

* Opening invoice emails
* Downloading PDF attachments
* Extracting invoice details
* Entering data into spreadsheets or accounting systems
* Tracking payment due dates
* Following up on unpaid invoices

This process is repetitive, time-consuming, and prone to human error.

## Solution

The AI Document Processing Agent automates the entire invoice processing workflow.

## Workflow

1. Gmail Trigger monitors incoming emails.
2. Email Classifier identifies invoice-related emails.
3. PDF invoices are extracted from email attachments.
4. AI extracts structured invoice information.
5. Duplicate invoice detection prevents duplicate records.
6. Invoice data is stored in Airtable.
7. Slack notifications alert the finance team.
8. Google Calendar reminders are scheduled before invoice due dates.
9. Payment status tracking monitors whether invoices are paid or pending.
10. Records are automatically updated throughout the invoice lifecycle.

## Features

### Invoice Email Classification

Automatically identifies invoice-related emails from incoming messages.

### AI-Powered Data Extraction

Extracts:

* Vendor Name
* Invoice Number
* Invoice Date
* Due Date
* Total Amount
* Tax Amount
* Payment Terms
* GST Number

### Duplicate Detection

Prevents duplicate invoices from being processed multiple times.

### Airtable Database

Stores structured invoice records for tracking and reporting.

### Slack Notifications

Sends real-time alerts when new invoices are processed.

### Payment Reminders

Creates calendar reminders before invoice due dates.

### Invoice Status Tracking

Tracks:

* Pending
* Paid
* Overdue

## Tech Stack

* n8n
* OpenRouter
* Gmail
* Airtable
* Slack
* Google Calendar
* AI Structured Output Parsing

## Sample Output

```json
{
  "vendor_name": "ABC Solutions",
  "invoice_number": "INV-2026-101",
  "invoice_date": "2026-06-15",
  "due_date": "2026-07-15",
  "total_amount": 29500,
  "tax_amount": 4500,
  "payment_terms": "Net 30"
}
```

## Business Value

* Reduces manual data entry
* Improves invoice processing speed
* Minimizes accounting errors
* Prevents duplicate payments
* Tracks upcoming payment deadlines
* Improves financial visibility

## Future Improvements

* OCR support for scanned invoices
* Automatic expense categorization
* Overdue invoice alerts
* Integration with accounting software
* Invoice approval workflows
* Analytics dashboard

## Author

Krish Dewangan

AI Automation Enthusiast | n8n Builder | Workflow Automation
