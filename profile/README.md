# Aqta

**AI Governance Platform**

Stop runaway costs, detect loops, and ensure compliance for AI systems.

## What is Aqta?

Aqta sits between your app and AI providers (OpenAI, Anthropic, Perplexity, etc.) to prevent runaway costs, detect infinite loops, and ensure compliance.

```
Your App → Aqta Gateway → AI Providers
               ↓
          Dashboard
```

## Quick Start

### 1. Sign Up
Visit [app.aqta.ai/signup](https://app.aqta.ai/signup)

### 2. Integrate
Works with any OpenAI-compatible API:

```python
# OpenAI
client = openai.OpenAI(
    api_key="sk-...",
    base_url="https://gateway.aqta.ai/v1"
)

# Anthropic
client = anthropic.Anthropic(
    api_key="sk-ant-...",
    base_url="https://gateway.aqta.ai/v1"
)

# Any OpenAI-compatible provider
base_url="https://gateway.aqta.ai/v1"
```

### 3. Monitor
View your dashboard at [app.aqta.ai](https://app.aqta.ai)

## Features

**Core:**
- Loop detection & prevention
- Multi-provider routing
- Cost tracking & optimisation
- Compliance audit trails

**Healthcare (Aqta Health):**
- Medical receipts (tamper-evident audit trails)
- Bias detection across demographics
- Human-in-the-loop workflows
- Patient portal
- HIPAA compliance

## Tech Stack

- **Gateway**: Python (FastAPI)
- **Dashboard**: Next.js 14
- **Database**: Supabase / Aurora DSQL
- **Deployment**: Vercel + Railway/Render

## Repository Structure

```
aqta/
├── gateway/          # Backend API (Python/FastAPI)
│   ├── app/
│   │   ├── main.py
│   │   ├── providers.py
│   │   └── healthcare/
│   └── migrations/
│
├── dashboard/        # Frontend (Next.js/React)
│   ├── app/
│   └── components/
│
└── docs/            # Documentation
```

## Local Development

```bash
# Gateway
cd gateway
pip install -r requirements.txt
cp .env.example .env
python -m app.main

# Dashboard
cd dashboard
npm install
cp .env.example .env.local
npm run dev
```

Access:
- Dashboard: http://localhost:3000
- API: http://localhost:8000

## Documentation

- [Quick Start](./docs/quick-start/README.md)
- [Healthcare Guide](./docs/guides/healthcare/README.md)
- [API Reference](./docs/api/README.md)
- [Deployment](./docs/deployment/README.md)

## Domains

- `aqta.ai` - Marketing
- `app.aqta.ai` - Dashboard
- `gateway.aqta.ai` - API Gateway

## Security

- HIPAA compliant
- GDPR ready
- End-to-end encryption
- Audit logging
- SOC 2 Type II (in progress)

## Support

- Email: hello@aqta.ai
- Status: [status.aqta.ai](https://status.aqta.ai)
- Pricing: [app.aqta.ai/pricing](https://app.aqta.ai/pricing)

## License

Proprietary. © 2026 Aqta. All rights reserved.

---

Built for AI governance and compliance
