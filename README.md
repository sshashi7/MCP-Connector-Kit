# Copilot Studio · MCP Connector Kit

Make any REST API callable by a Copilot Studio agent — in minutes, not days.

Configure your API, define your tools, pick an auth pattern, and the wizard
generates your MCP server files, walks you through deploying to Azure App Service,
and connects it to your Copilot Studio agent.

> ⚠️ Designed for PoC and demo use. See `PRODUCTION_READINESS.md` before going live.

---

## 🚀 Get started

Download `mcp-connector-kit.html` and open it in any modern browser.

No installation, no dependencies, no network required.

---

## 🧭 How it works

The wizard guides you through five things:

1. **Configure** — Name your server, enter your API base URL, set rate limits
2. **Define tools** — Describe what each endpoint does in natural language (this is what the agent reasons over)
3. **Choose auth** — 9 patterns supported: Entra ID Delegated, Service Principal, OAuth 2.0, Bearer, API Key, Basic, and more
4. **Generate** — Downloads a complete TypeScript MCP server project ready for `npm install`
5. **Deploy & connect** — Pre-filled Azure CLI commands and step-by-step Copilot Studio connection instructions

---

## 🔐 Auth patterns

The kit covers the full range of how APIs authenticate — from public APIs with no auth,
to user-delegated Entra ID flows with per-user audit trails, to service principal
app-to-app auth. The generated server includes the right middleware, token validation,
and `.env` structure for whichever pattern you choose.

---

## 📁 Files in this repo

| File | Purpose |
|------|---------|
| `mcp-connector-kit.html` | The wizard — open this |
| `PRODUCTION_READINESS.md` | Hardening checklist before going live |
| `LICENSE.md` | Usage terms — PoC and demo use only |
