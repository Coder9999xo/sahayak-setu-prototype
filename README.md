# 🇮🇳 Sahayak Setu: Voice-First Civic AI Agent

**Sahayak Setu** is an agentic AI platform designed to bridge the digital divide for rural India using the **Model Context Protocol (MCP)** and **Amazon Bedrock**.

## 🏗 Architecture
Our solution uses a "Glass Box" architecture to ensure transparency and trust:
- **Frontend:** Streamlit (Status-Driven UI)
- **Orchestrator:** AWS Lambda + Amazon Bedrock (Claude 3.5 Sonnet)
- **Voice Pipeline:** Amazon Transcribe (Input) -> Amazon Polly Neural (Output)
- **Tools (MCP):**
  - `identity_tool`: Fetches user data (Simulating DigiLocker/API Setu)
  - `browser_tool`: Headless navigation of government portals (Simulating Playwright)
  - `consent_tool`: Records verbal signatures to Amazon S3

## 🚀 Tech Stack
- **GenAI Model:** Anthropic Claude 3.5 Sonnet (Vision & Reasoning)
- **Cloud:** AWS (us-east-1)
- **Language:** Python 3.10+
- **Database:** DynamoDB (Session State)

## 📅 Roadmap
- [x] Architecture Design & MCP Schema Definition
- [x] UI/UX Wireframing (Glass Box Concept)
- [ ] Integration of Bedrock Knowledge Bases (RAG)
- [ ] "Verbal Signature" Logic Implementation
