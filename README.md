Add Cherry Studio quick-start sectionVX API — Developer Documentation

OpenAI-compatible API for DeepSeek, Qwen, GLM, Kimi and more. One API key. Many models. 40–70% cheaper than going direct.

- 🌍 Global access via Cloudflare edge network
- 💰 Pay-as-you-go, no minimum spend
- 🔑 Works with any OpenAI SDK — change one line of code
- ⚡ Simple sign-up, no enterprise contract

## Quick Start

### 1. Get your API key

Sign up at [https://api.vxvxvx.top](https://api.vxvxvx.top) and create a key from the dashboard.

### 2. Make your first request

**curl:**

```bash
curl https://api.vxvxvx.top/v1/chat/completions \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer YOUR_API_KEY" \
  -d '{
    "model": "deepseek-chat",
    "messages": [{"role": "user", "content": "Hello!"}]
  }'
```

**Python (openai SDK):**

```python
from openai import OpenAI

client = OpenAI(
    api_key="YOUR_API_KEY",
    base_url="https://api.vxvxvx.top/v1"
)

response = client.chat.completions.create(
    model="deepseek-chat",
    messages=[{"role": "user", "content": "Hello!"}]
)
print(response.choices[0].message.content)
```

**JavaScript / Node.js:**

```javascript
import OpenAI from "openai";

const client = new OpenAI({
    apiKey: "YOUR_API_KEY",
    baseURL: "https://api.vxvxvx.top/v1",
});

const response = await client.chat.completions.create({
    model: "deepseek-chat",
    messages: [{ role: "user", content: "Hello!" }],
});
console.log(response.choices[0].message.content);
```

That's it — if your code works with OpenAI, it works with VX API.

## Quick Start with Cherry Studio (No-Code)

[Cherry Studio](https://cherry-ai.com) is a desktop AI chat client. If you prefer a GUI over writing code, you can connect VX API to Cherry Studio in 3 minutes.

1. **Get an API key** from [https://api.vxvxvx.top](https://api.vxvxvx.top) (Dashboard → API Keys → Add Token).
2. **Download Cherry Studio** from [https://cherry-ai.com](https://cherry-ai.com), open it, and choose "Configure other providers".
3. **Add an OpenAI-compatible provider** with:
   - Name: `VX API`
   - API URL: `https://api.vxvxvx.top/v1`
   - API Key: your `sk-...` key
4. **Sync models**, pick `DeepSeek V4.1 Flash`, and start chatting.

For a full step-by-step guide with screenshots and troubleshooting, see [`VX_API_Cherry_Studio_图文接入指南.html`](./VX_API_Cherry_Studio_图文接入指南.html) in this repo.

**Common errors**
- `403 quota zero`: your key may be disabled or its quota stuck. Enable it in the dashboard, or create a new key with a fixed quota.
- `401 Failed to authenticate`: re-copy the full API key; make sure there are no spaces.
- `404 Not Found`: make sure the API URL ends with `/v1`.

## Supported Models

Chinese frontier models (our focus):

| Model | Best for |
|---|---|
| DeepSeek V4 series | General chat, coding, reasoning |
| Kimi K3 / K2.7-code | Long context, coding agents |
| Qwen 3.8-max | Multilingual, tool use |
| GLM 5.3 | Fast, cost-effective daily use |
| MiniMax M3 | Creative writing, long output |
| MiMo v2.5-pro | Lightweight tasks |

Also available: GPT, Claude, Grok, Gemini (via aggregation)

Full model list and live pricing: [https://api.vxvxvx.top/pricing](https://api.vxvxvx.top/pricing)

## Why developers choose VX API

- **Drop-in compatible** — keep your existing OpenAI SDK, just swap `base_url`
- **Built for indie devs & small teams** — burn tokens without burning your budget
- **Agent-friendly** — one key covers routing across models, auto-fallback keeps your agents running
- **Transparent pricing** — see the price calculator in the dashboard before you spend

## Links

- 🌐 Website & Dashboard: [https://api.vxvxvx.top](https://api.vxvxvx.top)
- 💬 Support: [2658687862@qq.com](mailto:2658687862@qq.com)
- 📖 Pricing: [https://api.vxvxvx.top/pricing](https://api.vxvxvx.top/pricing)
