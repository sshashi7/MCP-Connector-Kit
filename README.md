# Copilot Studio · MCP Connector Kit

Turn any REST API into an MCP tool your Copilot Studio agent can reason over — in minutes, not days.

Configure your API, define your tools, pick an auth pattern, and the wizard
generates your MCP server files, walks you through deploying to Azure App Service,
and connects it to your Copilot Studio agent.

> ⚠️ Designed for PoC and demo use. See `PRODUCTION_READINESS.md` before going live.

---

## 🚀 Get started

Download `mcp-connector-kit.html` and open it in any modern browser — the wizard guides you through the rest.

No installation, no dependencies, no network required.

---

## 🧭 How it works

The wizard has two paths:

<img width="700" height="390" alt="image" src="https://github.com/user-attachments/assets/6f2c13f0-d70e-4179-8f32-6458c939a710" />




**Learn first** — Start with a working sample using the Open Library public API.
Run live API calls in the browser, download the pre-built server files, deploy to Azure,
and connect to a Copilot Studio agent — end to end, before touching your own API.

**Build your MCP connector** — Eight guided steps for your own API:

1. **API details** — Enter your API base URL, connector name, and choose an auth pattern
2. **Define tools** — Describe each endpoint the agent can call — name, method, path, and parameters
3. **Security** — Configure your inbound key, or token validation for Entra flows
4. **Generate & download** — The wizard downloads your complete server project files: `server.ts`, `package.json`, `tsconfig.json`, `.env.example`, `.gitignore`, and `DEPLOYMENT.md`
5. **System check** — Verify Node 20+, Azure CLI, and Copilot Studio access are ready
6. **Deploy** — Run the pre-filled PowerShell commands to test locally, then deploy to Azure App Service with a single `az webapp up` command
7. **Connect to Copilot Studio** — The wizard generates step-by-step MCP connection instructions tailored to your auth type
8. **Test** — Enable generative orchestration and verify your tools with natural language

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
