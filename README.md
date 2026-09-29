# 🚀 Production-Grade n8n Automation & AI Workflows

A portfolio of production-ready automation pipelines engineered using **n8n**, **Google Gemini AI Models**, **REST APIs**, **Webhooks**, and **Discord**.

---

## 🛠 Projects Overview

### 1️⃣ Project #2: Multi-Tenant E-Commerce Inventory & Order Sync Engine
- **Core Stack:** n8n, Google Sheets, JavaScript Code Node, Gemini Chat Model
- **Key Features:**
  - Automated calculation of inventory stock variances across multi-tenant sheets.
  - Custom JavaScript logic to evaluate low-stock thresholds.
  - Real-time stock alert generation using AI.
- **Workflow JSON:** [`workflow/Project 2_ Multi-Tenant Inventory Sync.json`](./workflow)

### 2️⃣ Project #3: Automated Multi-Platform Social Media & Content Distribution Pipeline
- **Core Stack:** n8n, Google Gemini AI, Code Node (JSON Parser), HTTP Request Webhooks, Discord
- **Key Features:**
  - Ingests raw articles/posts and uses an AI Agent (`gemini-2.0-flash`) as a Content Marketing Director.
  - Formats output into platform-tailored LinkedIn posts, Twitter/X threads, and executive summaries.
  - Uses JavaScript parsing to handle dynamic JSON structures and routes payload under Discord's 2,000-character limits via HTTP POST webhooks.
- **Workflow JSON:** [`workflow/Project 3_ Content Distribution Pipeline.json`](./workflow)

### 3️⃣ Project #4: Enterprise Customer Support & AI Ticket Escalation System
- **Core Stack:** n8n, Webhook Trigger, AI Agent, If/Branching Nodes, Discord Webhooks
- **Key Features:**
  - Automated incoming ticket triage analyzing customer sentiment and assigning priority levels (`P1-Critical`, `P2-High`, `P3-Normal`).
  - Conditional branching logic (`If` nodes) to auto-generate customer responses for standard tickets while escalating `P1-Critical` issues directly to urgent Discord alert channels.
- **Workflow JSON:** [`workflow/Project 4_ Customer Support Escalation.json`](./workflow)

---

## 🔧 Architecture & Best Practices Implemented
- **Structured AI Outputs:** Enforced strict JSON output schemas from Gemini sub-nodes to eliminate unstructured text errors.
- **Error Handling & Limits:** Handled rate limits, character limits, and string escaping across API webhooks.
- **Production Data Parsing:** Custom JavaScript code execution for data transformation between n8n nodes.
