# Monet Voice Agent (ElevenLabs + Firecrawl)

## Overview
This project presents a **voice-based AI agent built with ElevenLabs** that acts as a virtual assistant for **Monet**, a Colombian fintech focused on microcredit access.

The agent is designed to:
- Answer user questions about Monet
- Educate users about financial services in simple terms
- Guide users toward next steps (exploration, onboarding, support)

It operates through **WhatsApp interaction** and leverages **real-time web scraping via Firecrawl** to ensure responses are grounded in up-to-date information from Monet’s website.

---

## 🔗 Live Demo

- **Try the agent (voice interface):**  
  https://elevenlabs.io/app/talk-to?agent_id=agent_5201kmk59q8gfgassab3a4tg4wes

- **Agent ID:**  
  `agent_5201kmk59q8gfgassab3a4tg4wes`

- **WhatsApp Test Line:**  
  +1 (555) 938-5414

---

## 🧠 Architecture

The system combines conversational AI, voice synthesis, and dynamic data retrieval:


User (WhatsApp / Voice)
↓
ElevenLabs Agent (Conversational Layer)
↓
LLM (Qwen3-30B-A3B)
↓
Firecrawl Tool (Web Scraping)
↓
Monet Website (https://www.monet.com.co
)


---

## ⚙️ Core Components

### 1. Conversational Agent (ElevenLabs)
- Platform: ElevenLabs
- Agent ID: `agent_5201kmk59q8gfgassab3a4tg4wes`
- Handles:
  - Dialogue flow
  - Voice interaction
  - Tool orchestration

---

### 2. LLM
- Model: **Qwen3-30B-A3B**
- Role:
  - Understand user intent
  - Generate responses in Spanish
  - Follow structured behavioral instructions (CRAFT framework)

---

### 3. Voice System
- Voice ID: `qHkrJuifPpn95wK3rm2A`
- Model: **Multilingual**
- Reason for selection:
  - Better performance in Spanish compared to v3
  - Natural, human-like tone

---

### 4. Firecrawl Integration (Tool)

The agent uses a custom tool powered by **Firecrawl** to retrieve real-time information.

- Endpoint:

POST https://api.firecrawl.dev/v2/scrape


- Functionality:
  - Performs a **full scroll scrape** of https://www.monet.com.co
  - Extracts structured content from the site
  - Enables the agent to answer based on **live website data**

---

## 🧩 Agent Behavior Design (CRAFT Framework)

The agent follows a structured prompt design:

### Context
- Monet is a fintech that provides digital financial solutions
- Focus: accessibility, simplicity, financial empowerment
- Users typically have:
  - Low familiarity with financial products
  - Curiosity or early-stage exploration

Key facts:
- 2.7M+ credits disbursed in Colombia
- 900K+ positive credit reports
- Gender-focused initiative: **"Mujer con M de Monet"**

---

### Role
The agent is **Andrea**, a virtual advisor:
- Trustworthy
- Clear and approachable
- Focused on education, not aggressive selling

---

### Actions
The agent is designed to:

1. **Identify user intent quickly**
2. **Explain Monet simply**
3. **Translate features into benefits**
4. **Guide next steps**
5. **Handle doubts and build trust**

---

### Response Format
- Short, conversational answers
- Maximum 2–3 key ideas per response
- Simple language (no financial jargon)

Structure:
1. Acknowledge intent  
2. Explain clearly  
3. Reinforce benefit  
4. Suggest next step  

---

### Tone
- Human and friendly
- Professional but not rigid
- Clear and empathetic
- Confident but never pushy

---

### Goal
Ensure that the user:
- Understands what Monet is
- Trusts the solution
- Feels comfortable taking the next step

---

## 💬 User Experience

The agent is designed for **WhatsApp-based conversations in Spanish**, enabling:

- Low-friction access
- Natural interaction
- Fast understanding of financial concepts

Example use cases:
- "What is Monet?"
- "How do I get a loan?"
- "Is this safe?"
- "Who is this for?"

---

## 🚀 Key Features

- ✅ Voice-enabled conversational agent  
- ✅ Real-time data retrieval via web scraping  
- ✅ Spanish-first experience  
- ✅ Financial education focus  
- ✅ WhatsApp-native interaction  
- ✅ Trust-building conversational design  

---

## 🧪 How to Test

### Option 1: Voice Interface
Use the ElevenLabs link:
https://elevenlabs.io/app/talk-to?agent_id=agent_5201kmk59q8gfgassab3a4tg4wes

### Option 2: WhatsApp
Send a message to:
+1 (555) 938-5414

---

## 📌 Notes

- The agent is designed to answer **simple and exploratory questions**
- It prioritizes **clarity over technical depth**
- If information is not available, it gracefully acknowledges limitations

---

## 🏁 Conclusion

This project demonstrates how combining:
- Conversational AI  
- Voice interfaces  
- Real-time web data  

can create a **scalable, user-friendly financial assistant** that improves accessibility and understanding in the fintech space.

---
