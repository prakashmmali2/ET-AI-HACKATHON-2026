# ET Guide AI

An AI-powered concierge prototype for the Economic Times (ET) ecosystem.
This project demonstrates how conversational AI can onboard users, profile their financial journey, and recommend ET products, services, and partner offerings.

---

## 🚀 Features

### ET Welcome Concierge

Smart onboarding with a short profiling conversation that maps users to ET Prime, ET Markets, ET Wealth, Masterclasses, and more.

### Financial Life Navigator

Guides users through their financial journey, identifying portfolio gaps and suggesting relevant ET tools.

### Cross-Sell Engine (Planned)

Proactive recommendations and upsell opportunities based on user behavior.

### Marketplace Concierge (Planned)

Conversational flows for credit cards, loans, insurance, and wealth management via ET partnerships.

---

## 🛠️ Tech Stack

Frontend: React + Vite
Backend (planned): Node.js / Express
State Management: React Context / Redux (future upgrade)
AI Layer: OpenAI / LangChain (planned integration)
Deployment: Netlify

---

## 📂 Project Structure

et-guide-ai/
│── public/              # Static assets
│── src/
│   ├── components/      # UI components (chat, onboarding, recommendations)
│   ├── services/        # API integration & recommendation logic
│   ├── utils/           # Helper functions
│   ├── App.js           # Main entry point
│   └── index.js         # React bootstrap
│── README.md            # Project overview
│── Documentation.md     # Detailed technical documentation

---

## ⚡ Getting Started

### 1. Clone the repo

```bash
git clone https://github.com/prakashmmali2/et-guide-ai.git
cd et-guide-ai
```

### 2. Install dependencies

```bash
npm install
```

### 3. Run locally

```bash
npm run dev
```

### 4. Build for production

```bash
npm run build
```

---

## 🔗 Live Demo

ET Guide AI Prototype

---

## 📌 Roadmap

[x] Basic onboarding & product mapping

[x] Deeper financial profiling

[x] Cross-sell & upsell engine

[x] Partner API integration for marketplace services

[x] Voice + chat support

---

## 🤝 Contributing

Pull requests are welcome. For major changes, open an issue first to discuss the proposed updates.

---

## 📜 License

MIT License

---

# ET Guide AI - Technical Documentation

This section provides a deeper explanation of the architecture, workflows, and optimization strategies.

---

## 1. System Overview

ET Guide AI is designed as a conversational concierge that:

* Profiles users in under 3 minutes.
* Maps them to ET ecosystem products.
* Provides financial navigation and partner services.
* Learns continuously from user behavior.

---

## 2. Architecture

### Current Flow

1. User Onboarding → Profiling questions (investment journey, goals)
2. Recommendation Engine → Maps profile to ET Prime, ET Markets, ET Wealth
3. Portfolio Analyzer (optional) → Suggests improvements
4. Static Marketplace Listing → Shows partner services

### Planned Flow

Adaptive Dialogue Engine (NLP + LangChain)
Cross-Sell Engine (event-driven triggers)
Marketplace Concierge (API integration for loans, insurance, credit cards)
Persistent User Profiles (stored in database and updated dynamically)

---

## 3. Code Efficiency Improvements

State Management
Move from local state to Redux or Zustand for global persistence.

Recommendation Engine
Replace hardcoded mappings with rule-based plus ML hybrid logic.

API Calls
Use async batching and caching to reduce latency.

Component Optimization
Apply React.memo and useCallback to prevent unnecessary re-renders.

Progressive Profiling
Collect user data gradually across sessions rather than a single onboarding step.

---

## 4. Deployment

Frontend
Netlify with CI/CD pipelines.

Backend (future)
Node.js + Express REST APIs.

Database (future)
MongoDB for user profiles and analytics.

Analytics
Kafka or PubSub for event-driven triggers.

---

## 5. Roadmap

Phase 1 (Current)
Basic onboarding and static recommendations.

Phase 2
Financial Life Navigator with portfolio gap analysis.

Phase 3
Cross-sell engine with predictive modeling.

Phase 4
Marketplace concierge with partner API integration.

Phase 5
Voice and chat support with continuous learning.

---

## 6. Contribution Guidelines

* Fork the repository and create a feature branch.
* Write modular, well-documented code.
* Ensure pull requests include tests and documentation updates.
* Follow ESLint and Prettier formatting rules.

🔗 Live Demo
👉 [ET Guide AI Prototype](https://et-guide-ai.lovable.app/)
