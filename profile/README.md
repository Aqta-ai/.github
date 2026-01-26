# Aqta

**System of Record for AI Agents**

Aqta is an AI governance platform that prevents runaway costs, detects infinite loops and ensures compliance for AI systems.

---

## 🚀 What is Aqta?

Aqta sits between your application and AI providers (OpenAI, Anthropic, Google, etc.) to:

- **Stop runaway costs** before they happen
- **Detect infinite loops** in real-time
- **Route intelligently** across multiple AI providers
- **Monitor compliance** for regulated industries
- **Ensure patient safety** in healthcare AI (Aqta Health)

---

## 🏥 Aqta Health

Healthcare-specific AI governance:

- **Medical Receipts**: Tamper-evident audit trails for every AI decision
- **Bias Detection**: Monitor fairness across demographics (age, gender, race, SES)
- **Human-in-the-Loop**: Route high-risk decisions to human reviewers
- **Patient Portal**: Transparent AI records for patients
- **HIPAA Compliance**: Built for healthcare from day one

## 🛠️ Architecture

```
Your App → Aqta Gateway → AI Providers (OpenAI, Anthropic, etc.)
              ↓
         Dashboard (app.aqta.ai)
```

**Domains:**
- `aqta.ai` - Marketing site
- `app.aqta.ai` - Dashboard (auth required)
- `gateway.aqta.ai` - API Gateway

**Tech Stack:**
- Gateway: Python (FastAPI)
- Dashboard: Next.js 14 (App Router)
- Database: Supabase (PostgreSQL) or Aurora DSQL
- Deployment: Vercel (dashboard) + Railway/Render (gateway)

---

## 📦 Quick Start

### 1. Sign Up
Visit [app.aqta.ai/signup](https://app.aqta.ai/signup) to create an account.

We'll provision your API key within 48 hours (manual provisioning prevents abuse).

### 2. Integrate

Replace your OpenAI endpoint:

```python
# Before
import openai
client = openai.OpenAI(api_key="sk-...")

# After
import openai
client = openai.OpenAI(
    api_key="aqta_live_...",  # Your Aqta API key
    base_url="https://gateway.aqta.ai/v1"
)
```

That's it! All your AI requests now flow through Aqta.

### 3. Monitor

View your dashboard at [app.aqta.ai](https://app.aqta.ai):
- Real-time cost tracking
- Loop detection alerts
- Request volume charts
- Model usage breakdown

---

## 🏥 Healthcare Quick Start

For healthcare AI systems:

1. **Book a demo**: [aqta.ai/healthcare](https://aqta.ai/healthcare)
2. **Custom onboarding**: We'll configure bias detection, HITL workflows, and compliance settings
3. **Integrate**: Same API, healthcare features enabled automatically
4. **Monitor**: View medical receipts, bias trends, and review workflows at [app.aqta.ai/healthcare](https://app.aqta.ai/healthcare)

---

## 🔒 Security & Compliance

- **HIPAA Compliant**: Healthcare data handling meets HIPAA requirements
- **GDPR Ready**: EU data residency and privacy controls
- **SOC 2 Type II**: In progress
- **ISO 27001**: Planned for 2026

**Security Features:**
- End-to-end encryption
- Audit logging
- Role-based access control
- Session management
- API key rotation

---

## 💰 Pricing

[View full pricing →](https://aqta.ai/pricing)

---

## 🌍 Sustainability (Green AI)

By preventing redundant agent loops and runaway inference, Aqta directly reduces wasted compute and associated energy consumption.

**Impact:**
- Prevent unnecessary AI requests
- Optimise model selection (use smaller models when possible)
- Cache responses intelligently
- Stop infinite loops before they waste energy

---

## 🤝 Support

- **Email**: hello@aqta.ai
- **Documentation**: [docs.aqta.ai](https://docs.aqta.ai)
- **Status**: [status.aqta.ai](https://status.aqta.ai)

---

## 📜 License

**Proprietary. Copyright © 2026 Aqta. All rights reserved.**

This is closed-source software. Contact us for licensing inquiries.

---

## 🔗 Links

- **Website**: [aqta.ai](https://aqta.ai)
- **Demo**: [demo.aqta.ai](https://demo.aqta.ai)
- **Dashboard**: [app.aqta.ai](https://app.aqta.ai)
- **Healthcare**: [aqta.ai/healthcare](https://aqta.ai/healthcare)

---

**Built with ❤️ for AI governance and compliance**
