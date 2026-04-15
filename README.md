<div align="center">

# NeuronGate

### One API. Every Model. Pay with Crypto.

[![Website](https://img.shields.io/badge/Website-neurongate.net-6366f1?style=for-the-badge&logo=globe&logoColor=white)](https://neurongate.net)
[![API Status](https://img.shields.io/badge/API_Status-Operational-10b981?style=for-the-badge&logo=statuspage&logoColor=white)](https://neurongate.net)
[![Models](https://img.shields.io/badge/Models-50+-8b5cf6?style=for-the-badge&logo=brain&logoColor=white)](https://neurongate.net/models)

---

**NeuronGate** is a unified AI API gateway that gives you access to **50+ models** from every major provider through a single, OpenAI-compatible endpoint. No vendor lock-in. No credit cards. Just crypto and code.

</div>

## 🔑 Why NeuronGate?

| Feature | Description |
|---------|-------------|
| **🔀 One API, Every Model** | Access OpenAI, Anthropic, Google, Meta, Mistral, DeepSeek, Cohere, xAI — all through `neurongate.net/v1` |
| **💰 Crypto Payments** | Pay with USDT, USDC, ETH, or BTC. No credit card. No KYC for basic access. |
| **🔌 OpenAI-Compatible** | Drop-in replacement — change your base URL, keep your code |
| **📊 Built-in Analytics** | Real-time usage tracking, spend monitoring, per-key breakdowns |
| **🔑 Multi-Key Management** | Create scoped API keys for different projects, teams, or environments |
| **⚡ Automatic Failover** | If a provider goes down, requests route to the next best model |

## ⚡ Quickstart

```bash
# That's it. Change the base URL, keep everything else.
curl https://neurongate.net/v1/chat/completions \
  -H "Authorization: Bearer ng-your-api-key" \
  -H "Content-Type: application/json" \
  -d '{
    "model": "openai/gpt-4o",
    "messages": [{"role": "user", "content": "Hello!"}]
  }'
```

```python
from openai import OpenAI

client = OpenAI(
    base_url="https://neurongate.net/v1",
    api_key="ng-your-api-key"
)

response = client.chat.completions.create(
    model="anthropic/claude-sonnet-4-6",
    messages=[{"role": "user", "content": "Explain quantum computing"}]
)
print(response.choices[0].message.content)
```

## 🧠 Supported Providers

<table>
<tr>
<td align="center"><b>OpenAI</b><br/>GPT-4o, GPT-4.1, GPT-5, o1, o3</td>
<td align="center"><b>Anthropic</b><br/>Claude Opus 4.6, Sonnet 4.6, Haiku 4.5</td>
<td align="center"><b>Google</b><br/>Gemini 2.5 Pro, Flash, Ultra</td>
<td align="center"><b>Meta</b><br/>Llama 4, Llama 3.3, Maverick</td>
</tr>
<tr>
<td align="center"><b>Mistral</b><br/>Large, Medium, Codestral</td>
<td align="center"><b>DeepSeek</b><br/>V3, R1, Coder</td>
<td align="center"><b>Cohere</b><br/>Command R+, Embed</td>
<td align="center"><b>xAI</b><br/>Grok 3, Grok 3 Mini</td>
</tr>
</table>

**→ [Browse all 50+ models](https://neurongate.net/models)**

## 💳 Pricing

No subscriptions. No minimums. Pay for what you use.

- **Top up** with USDT, USDC, ETH, or BTC
- **Same rates** as direct provider pricing (often cheaper)
- **Real-time** balance tracking in your dashboard
- **Detailed invoices** for every payment

**→ [View pricing calculator](https://neurongate.net/#pricing)**

## 📚 Resources

| Resource | Link |
|----------|------|
| 📖 API Documentation | [neurongate/docs](https://github.com/neurongate/docs) |
| 💻 Code Examples | [neurongate/examples](https://github.com/neurongate/examples) |
| 🌐 Website | [neurongate.net](https://neurongate.net) |
| 🔑 Get API Key | [neurongate.net/keys](https://neurongate.net/keys) |

## 🔒 Security

- **TLS 1.2/1.3** encryption on all endpoints
- **No data retention** — we don't store your prompts or completions
- **Scoped API keys** — limit access per key
- **Rate limiting** — built-in DDoS protection
- **HTTPS only** — HTTP auto-redirects to HTTPS

---

<div align="center">

**[Get Started →](https://neurongate.net/login?register=true)** · **[Read the Docs →](https://github.com/neurongate/docs)** · **[Browse Models →](https://neurongate.net/models)**

<sub>Built for developers who want freedom of choice.</sub>

</div>
