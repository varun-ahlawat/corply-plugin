# Authentication

Use this only when Corply tools are unavailable or report that authentication is missing. Never ask
for an access token, cookie, credential, or private backend URL.

## Claude Code plugin

Run:

```bash
claude mcp login plugin:corply:corply
```

Tell the founder that their browser is opening so they can sign in with Google and link Claude Code
to Corply. On Claude Code versions before `claude mcp login`, direct them to `/mcp`, choose
**corply**, and complete browser sign-in.

## Codex or ChatGPT plugin

Ask the founder to open **Plugins**, choose **Corply**, and select **Connect** or **Reconnect**. If
the current task still cannot see the connected tools, start a new task after connecting.

## Direct Codex CLI MCP setup

Run:

```bash
codex mcp login corply
```

After authentication, retry the blocked read once. If the active process still does not see the
connection, explain that a fresh agent session is required; do not restart the company workflow or
create duplicate state.
