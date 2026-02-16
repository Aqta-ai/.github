# Aqta

**Agentic Security Infrastructure**  
Stop runaway costs, detect loops, and ensure governance for AI systems.

## What is Aqta?

Aqta sits between your app and AI providers (OpenAI, Anthropic, Perplexity, etc.) to prevent runaway costs, detect infinite loops, and ensure governance.

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

- **Loop Detection** - Automatically detect and prevent infinite loops
- **Cost Tracking** - Monitor and optimise AI API costs
- **Multi-Provider** - Works with OpenAI, Anthropic, Google, Perplexity
- **Governance** - Audit trails and compliance reporting
- **Network Intelligence** - Advanced threat detection (Team plan)

## Documentation

- [Get Started](https://app.aqta.ai/signup) - Create your free account
- [View Demo](https://app.aqta.ai/demo) - See Aqta in action
- [Pricing](https://app.aqta.ai/pricing) - Plans and features

## Support

- **Website:** [aqta.ai](https://aqta.ai)
- **Email:** hello@aqta.ai
- **Status:** [app.aqta.ai/status](https://app.aqta.ai/status)

## License

Proprietary. © 2026 Aqta Technologies Ltd. All rights reserved.

---

**Built for agentic security and AI governance**
