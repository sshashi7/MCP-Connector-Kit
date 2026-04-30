# MCP Connector Kit — Copilot Studio Integration

⚠️ **FOR PROOF-OF-CONCEPT AND DEMO USE ONLY**

---

## What Is This?

An interactive tool that generates TypeScript MCP (Model Context Protocol) servers for Copilot Studio. It lets Copilot Studio agents call your REST API as a tool — with proper authentication, error handling, and deployment to Azure.

**Input:** Your API details (base URL, credentials, endpoints)  
**Output:** Ready-to-deploy TypeScript server code

---

## Why Use It?

- **No boilerplate** — Skip weeks of MCP server setup
- **Test real APIs** — Includes guided walkthroughs with GitHub/Spotify-style APIs
- **Safe for PoC** — All code runs locally; credentials never leave your browser
- **Works everywhere** — Deploy to Azure, AWS, GCP, or anywhere Node.js runs

---

## How to Get Started

### 1. Open the Tool
Download and open `mcp-connector-kit.html` in any modern browser:

```bash
# Windows PowerShell
start mcp-connector-kit.html

# Mac
open mcp-connector-kit.html

# Linux
firefox mcp-connector-kit.html
```

Works completely offline. No installation needed.

### 2. Choose Your Path
- **Path A: Learn First** — Generate a connector using a free test API (GitHub, Spotify, etc.)
- **Path B: Your API** — Jump straight to your own test API

### 3. Configure & Generate
1. Enter your API details (base URL, test credentials only)
2. Select endpoints Copilot should be able to call
3. Choose authentication type (Bearer token, API key, OAuth, etc.)
4. Download the generated TypeScript project

### 4. Deploy & Test
```bash
# Local testing
npm install
npm run dev

# Deploy to Azure
az webapp up

# Connect to Copilot Studio agent and test
```

---

## 🚀 Quick Path (3 Steps)

1. **Open:** `mcp-connector-kit.html` in your browser
2. **Configure:** Fill in test API details, choose endpoints, select auth
3. **Deploy:** Run locally or push to Azure

---

## 📋 Files in This Kit

| File | Purpose |
|------|---------|
| **mcp-connector-kit.html** | Interactive generator — configure & generate your MCP server |
| **MCP_API_Setup_Guide.docx** | Test guide — hands-on examples using GitHub/Spotify-style APIs |
| **LICENSE.md** | Usage terms and restrictions (PoC/demo only) |
| **PRODUCTION_READINESS.md** | Security checklist for production deployment |
| **README.md** | This file |

---

## Key Safety Guidelines

✅ **Use test/demo credentials only** — Never enter production API keys  
✅ **Review generated code** — Inspect before deploying  
✅ **Store credentials in `.env`** — Keep out of version control  
✅ **Clean up after testing** — Delete Azure resources and credentials  
✅ **Check PRODUCTION_READINESS.md** — Required for any production use  

---

## What This Kit Includes

- ✅ MCP server boilerplate (TypeScript)
- ✅ Authentication templates (Bearer, API Key, OAuth, Basic, Entra ID, SharePoint)
- ✅ Environment variable support
- ✅ Basic error handling and health checks
- ✅ Azure App Service deployment guide

---

## What This Kit Does NOT Include (Add for Production)

- ❌ Rate limiting enforcement
- ❌ Secrets management (Azure Key Vault)
- ❌ Audit logging
- ❌ Request validation/sanitization
- ❌ CORS policies
- ❌ Load balancing / high availability
- ❌ Encryption at rest
- ❌ Compliance controls (SOC 2, HIPAA, etc.)

**Production requires 5-9 weeks of hardening.** See [PRODUCTION_READINESS.md](./PRODUCTION_READINESS.md) for the complete checklist.

---

## How the Tool Works

1. **Your browser only** — All code generation happens locally; credentials never leave your machine
2. **No external calls** — Completely offline after loading
3. **Inspect the source** — Open mcp-connector-kit.html in any text editor to verify

---

## Support & Questions

| Question | Answer |
|----------|--------|
| **Any REST API?** | Yes — Bearer token, API Key, OAuth, Basic auth, Entra ID, SharePoint |
| **Deploy to AWS/GCP?** | Yes — Node.js runs anywhere |
| **Custom authentication?** | Yes — Generated code is fully customizable |
| **Ready for production?** | No — This is PoC/demo only |
| **Support available?** | No — As-is, no SLA |

See [LICENSE.md](./LICENSE.md) for full terms.

---

## 🚀 Next Steps

1. **Get started** → Open `mcp-connector-kit.html` now
2. **Test first** → Use [MCP_API_Setup_Guide.docx](./MCP_API_Setup_Guide.docx) examples before your own API
3. **Going to production?** → Review [PRODUCTION_READINESS.md](./PRODUCTION_READINESS.md)

---

## Important Notes

- ⚠️ **This is a PoC/demo kit only** — Not suitable for production without significant hardening
- ⚠️ **Never use production credentials** — Only test/demo credentials during development
- ⚠️ **Clean up resources** — Delete all test credentials and Azure resources after testing

For production deployment, see [PRODUCTION_READINESS.md](./PRODUCTION_READINESS.md) — mandatory 5-9 week security hardening required.

---

**Ready to demo?** Open `mcp-connector-kit.html` in your browser now! 🚀
