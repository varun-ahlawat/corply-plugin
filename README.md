# Corply — incorporate your startup from Claude Code

Corply is your startup's AI **general counsel**. Install the plugin, sign in once, and form a
Delaware C-corp end-to-end — guided application, generated documents, conversational e-signature,
and filing handoff — without leaving Claude Code.

## Install

```
claude plugin marketplace add varun-ahlawat/corply-plugin
claude plugin install corply
```

Then run `/incorporate`. On the first tool call your browser opens once to sign in with Google;
after that Claude Code is authorized into your organization.

## What it does

- **Guided application** — the agent gathers structure, name, founders, ownership, equity terms,
  roles, 83(b), and tax info in one pass, and advises on standard choices.
- **Documents** — Certificate of Incorporation, Bylaws, Action of Incorporator, Board Consent.
- **Conversational e-signature** — you review each PDF via a magic link, then sign in-chat under
  ESIGN/UETA with a full audit trail. The only thing that happens on the web is reviewing the PDF.
- **Cofounders** — invite them by email; they sign from their own Claude Code and land in the same
  org automatically.
- **Filing** — Corply files with Delaware after everyone signs.

## How it works

This repo is **just the plugin** — a thin client. All logic runs on Corply's hosted MCP server
(`.mcp.json` → `https://corply.dev/mcp`); no company data, code, or credentials live here.

---

**Corply is operated by 0Lumen Labs Corp. Corply is not a law firm and does not provide legal advice.**
