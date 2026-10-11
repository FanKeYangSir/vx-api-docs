VX API — Developer Documentation
OpenAI-compatible API for DeepSeek, Qwen, GLM, Kimi and more.
One API key. Many models. 40–70% cheaper than going direct.

🌍 Global access via Cloudflare edge network
💰 Pay-as-you-go, no minimum spend
🔑 Works with any OpenAI SDK — change one line of code
⚡ Simple sign-up, no enterprise contract
Quick Start
1. Get your API key
Sign up at https://api.vxvxvx.top and create a key from the dashboard.

2. Make your first request
curl:

curl https://api.vxvxvx.top/v1/chat/completions \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer YOUR_API_KEY" \
  -d '{
    "model": "deepseek-chat",
    "messages": [{"role": "user", "content": "Hello!"}]
  }'
Python (openai SDK):

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
JavaScript / Node.js:

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
That's it — if your code works with OpenAI, it works with VX API.

Supported Models
Chinese frontier models (our focus):

Model	Best for
DeepSeek V4 series	General chat, coding, reasoning
Kimi K3 / K2.7-code	Long context, coding agents
Qwen 3.8-max	Multilingual, tool use
GLM 5.3	Fast, cost-effective daily use
MiniMax M3	Creative writing, long output
MiMo v2.5-pro	Lightweight tasks
Also available: GPT, Claude, Grok, Gemini (via aggregation)

Full model list and live pricing: https://api.vxvxvx.top/pricing

Why developers choose VX API
Drop-in compatible — keep your existing OpenAI SDK, just swap base_url
Built for indie devs & small teams — burn tokens without burning your budget
Agent-friendly — one key covers routing across models, auto-fallback keeps your agents running
Transparent pricing — see the price calculator in the dashboard before you spend
Links
🌐 Website & Dashboard: https://api.vxvxvx.top
💬 Support: 2658687862@qq.com
📖 Pricing: https://api.vxvxvx.top/pricing
