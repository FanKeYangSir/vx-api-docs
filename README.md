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
- `403 用户额度不足 / quota zero`: your key may be disabled or its quota stuck. Enable it in the dashboard, or create a new key with a fixed quota.
- `401 Failed to authenticate`: re-copy the full API key; make sure there are no spaces.
- `404 Not Found`: make sure the API URL ends with `/v1`.
