# 🚀 Yash-Singh-Nutrabay-Submission

An AI-powered system that converts raw SOP documents into structured summaries, training modules, quizzes, and automatically generated presentation slides — all delivered through a modern web interface.

---
<img width="1858" height="753" alt="image" src="https://github.com/user-attachments/assets/ead29735-f01a-4331-9eb5-375f63554adf" />

## 🧠 Overview

This project automates the transformation of unstructured content (text/files) into high-quality learning material using AI and workflow automation.

It processes SOPs (Standard Operating Procedures) and generates:

- 📌 Structured summaries  
- 📚 Step-by-step training content  
- 🧩 Interactive quizzes  
- 🎞️ Professional presentation slides (PDF + editable link)

---

## ✨ Features

### 🤖 AI Content Generation
- Converts raw text or files into structured JSON
- Ensures high-quality and complete coverage of content
- Handles large and complex SOPs

### 📖 Training Module Creation
- Step-by-step structured learning flow
- Clear explanations for easy understanding
- Designed for onboarding & training use cases

### 🧩 Quiz Generation
- Auto-generated MCQ-based questions
- Includes:
  - Options
  - Correct answer
  - Explanation

### 🎞️ Presentation Generation
- Automatically creates slides using Presenton
- Asynchronous generation with polling
- Outputs:
  - Downloadable PDF
  - Editable presentation link

### 🌐 Modern UI
- Accepts:
  - Text input
  - File upload
  - File + text
- Displays:
  - Summary
  - Training steps
  - Quiz interaction
  - Embedded PDF slide viewer

---

## ⚙️ Workflow Architecture

```text
User Input (UI)
   ↓
Webhook Trigger (n8n)
   ↓
AI Agent (Generate Structured JSON)
   ↓
Code Node (Parse & Clean JSON)
   ↓
Presenton (Generate Slides - Async)
   ↓
Polling Loop (Wait until completed)
   ↓
Merge Data (Content + Slides)
   ↓
Webhook Response
   ↓
Frontend Rendering
