# Tax Agency AI Lead Engine — AI Automation System

## 🚀 Overview
This project is an AI-powered lead processing and qualification system built using n8n. It automates the entire workflow of capturing client leads, analyzing their issues using AI, scoring lead quality, and sending automated email notifications.

The system is designed for tax agencies to instantly understand client needs and respond faster with intelligent follow-ups.

---

## 🎯 Problem Statement
Tax agencies receive client inquiries through forms, but manually reviewing each lead, understanding the issue, and responding takes time and leads to delays.

This results in:
- Slow response times
- Missed high-value clients
- Inefficient lead prioritization

---

## ⚙️ Solution
This workflow fully automates lead handling from intake to response:

- Captures new leads from Google Forms → Google Sheets
- Cleans and structures incoming data
- Uses AI (Groq API) to summarize client issues
- Generates a lead score using JavaScript logic
- Stores enriched lead data in a separate Google Sheet
- Sends automated follow-up email to client
- Sends instant alert email to agency team

---

## 🧠 Workflow Architecture

Google Form → Google Sheets Trigger → Data Cleaning → AI Processing (Groq API) → Lead Scoring (JS Code Node) → Output Google Sheet → Email Automation

---

## 🔧 Tech Stack
- n8n (Workflow Automation Engine)
- Google Sheets API
- Google Forms
- Groq AI API (LLM for summarization)
- Gmail API
- JavaScript (Lead scoring logic)
- Webhooks / HTTP Requests

---

## 📦 Features
- Real-time lead capture from forms
- AI-powered issue summarization
- Automated lead scoring system
- Smart lead prioritization
- Dual email automation (client + agency)
- Fully hands-free workflow

---

## 🧠 How It Works

### 1. Lead Capture
A new client submits a Google Form → data is stored in Google Sheets

### 2. Trigger
n8n detects new row in Google Sheet and starts workflow

### 3. Data Cleaning
Raw input is cleaned and structured for processing

### 4. AI Processing
Groq API analyzes the client's issue and generates:
- Summary of problem
- Key concern extraction

### 5. Lead Scoring (JavaScript Node)
A scoring system evaluates lead quality based on:
- Urgency
- Complexity
- Business value

### 6. Data Storage
Processed data is saved into a separate Google Sheet for tracking

### 7. Email Automation
- Client receives follow-up email acknowledging their request
- Agency receives alert email with:
  - Lead summary
  - Lead score
  - Issue severity

---

## 📸 Demo

### Input Example
Client submits tax-related query via Google Form

### Output Example
- AI Summary: "Client is facing issues with GST filing deadline..."
- Lead Score: 85/100 (High Priority)

---

## 📈 Real-World Impact
- Reduces manual lead review time by 80–90%
- Improves response time to clients
- Helps agencies prioritize high-value leads
- Automates repetitive administrative tasks

---

## 🚀 How to Use

1. Import workflow JSON into n8n
2. Connect Google Sheets credentials
3. Set up Groq API key in HTTP node
4. Configure Gmail credentials
5. Activate workflow
6. Submit a test Google Form entry

---

## 👨‍💻 Author
Built by {{Your Name}} — AI Automation Builder specializing in n8n workflow systems, API integrations, and business automation solutions.
