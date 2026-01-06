# Aqta

**Governance at the speed of AI.**  
The runtime governance layer for enterprise AI agents.

Aqta is a **Governance Gateway** that sits between your application and LLM providers. It stops loop drift, enforces spend caps, and automates EU AI Act compliance (Article 12 & 72) with **zero code changes** to your agents.

---

## 🚀 Features

### Runtime Protection (Active Defense)
*   **Loop Detection:** Automatically detects and suppresses runaway agent loops (e.g., repeating the same tool call 5x) before they drain your budget.
*   **Circuit Breakers:** Set hard limits on **Cost per Request**, **Steps per Trace**, or **Tokens per User**.
*   **Policy Engine:** Enforce governance rules (e.g., "No GPT-4 for internal dev environments") centrally.

### Compliance & Observability
*   **Immutable Audit Logs:** Every request, decision, and tool output is logged with a unique `trace_id`. Designed for **EU AI Act Article 12** auditability.
*   **Real-time Dashboard:** Monitor agent spend, latency, and violations in real-time.
*   **Human-in-the-Loop:** Flag suspicious traces for manual review by compliance teams.

### Universal Compatibility
*   **Drop-in Proxy:** Compatible with any OpenAI-compliant SDK (LangChain, CrewAI, Vercel AI SDK, etc.).
*   **Multi-Provider:** Route requests to OpenAI, Anthropic, or local models while maintaining a single governance layer.

---

## 🛡️ Why Aqta?

### The Problem: Loop Drift
Agentic AI is non-deterministic. Agents can get stuck in "loops"—repeating actions that burn through budget and API limits. Traditional observability tools only show you the bill *after* the incident.

### The Solution: Active Governance
Aqta is not just a logger; it is a **firewall**. It actively intervenes to stop bad behavior at runtime.

| Feature | Passive Observability (Datadog/LangSmith) | Active Governance (Aqta) |
| :--- | :--- | :--- |
| **Loop Detection** | Alert after 10 mins | **Block request immediately** |
| **Cost Control** | Monthly budget alert | **Per-request circuit breaker** |
| **Compliance** | Log storage | **Policy enforcement** |

---

## 🌍 Sustainability (Green AI)
By preventing redundant agent loops and runaway inference, Aqta directly reduces wasted compute and associated energy consumption.

---

## 🤝 Contributing
Aqta is currently in **Private Beta**.
To become a design partner or request features, please email [contact@aqta.dev](mailto:contact@aqta.dev).

---

## 📜 License
Proprietary. Copyright © 2026 Aqta AI Governance Limited. All rights reserved.
