# 🧠 Sentinel Explain Dashboard

**Sentinel Explain** is a prototype dashboard designed to analyze text for potential phishing, scam, or security threat indicators.  
It provides heuristic-based scoring, contextual explanations, and suggested actions — simulating how an AI-assisted SOC (Security Operations Center) tool might interpret suspicious messages.

---

## 🚀 Features

- **Real-time Threat Analysis:**  
  Paste or type any message (email, text, or alert) to get an instant threat score.

- **Dynamic Heuristic Scoring:**  
  Keyword and context-aware detection for phrases like _"password"_, _"urgent"_, _"document"_, and others.

- **Contextual Weighting:**  
  Scores adjust based on proximity of high-risk terms — for example, “urgent” near “review” or “document” increases suspicion.

- **Visual Threat Feedback:**  
  Color-coded alerts for quick interpretation of severity.

- **Suggested Actions:**  
  Simple guidance like “Mark as Safe” or “Run Full Analysis” (demo only).

---

## 🧩 Tech Stack

- **React + Vite** – for a fast, modern frontend  
- **Tailwind CSS** – for styling and color theming  
- **Lucide Icons / ShadCN UI** – for clean UI components  
- **Framer Motion (optional)** – for subtle animations

---

## 🧠 How It Works

The dashboard runs a lightweight heuristic engine (`analyzeText()`) that:
1. Parses the input text
2. Matches high-risk keywords and patterns  
3. Weighs their context (e.g., “urgent” near “document”)  
4. Computes a dynamic threat **score** (0–100)
5. Displays an explanation and suggested action

> ⚙️ The logic is rule-based for now — future iterations can integrate ML models or connect to external APIs for live threat scoring.

---

## 💻 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/<your-username>/sentinel-explain-dashboard.git
cd sentinel-explain-dashboard
