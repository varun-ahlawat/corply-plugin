# Authentication

Use this only when Corply tools are unavailable or report that authentication is missing. Never ask
for an access token, cookie, credential, or private backend URL.

If Corply reports expired, missing, invalid, or revoked authentication—or
`TERMS_ACCEPTANCE_REQUIRED`—reconnect using the surface-specific flow below, complete any required
browser step, then retry the blocked read once. Do not try to bypass or record terms acceptance
through ordinary company tools.

## Claude Code plugin

For expired, missing, invalid, or revoked authentication, briefly tell the founder: "Your Corply
login has expired. I’m reopening sign-in now—finish Google sign-in in the browser." For
`TERMS_ACCEPTANCE_REQUIRED`, say instead: "Corply needs you to accept the current terms. I’m
reopening sign-in now—review them in the browser."

Immediately run this command yourself with Claude Code's normal Bash tool and background execution
enabled:

```bash
claude mcp login plugin:corply:corply
```

Do not ask the founder to type the command or ask whether you should run it. Let Claude Code display
its normal shell-approval prompt when the current permission mode requires one. Do not wrap the
command in `script`, `nohup`, shell control operators, or another pseudo-terminal command. Monitor
the background command and retry the blocked Corply read once it succeeds.

Only after the automatic attempt fails may you show the founder the command to run manually. If the
failure proves that `claude mcp login` is unavailable on an older Claude Code version, direct them
to `/mcp`, choose **corply**, and complete browser sign-in.

## Codex or ChatGPT plugin

Ask the founder to open **Plugins**, choose **Corply**, and select **Connect** or **Reconnect**. If
the current task still cannot see the connected tools, start a new task after connecting.

## Direct Codex CLI MCP setup

Briefly explain that Corply needs to reconnect, then run this yourself:

```bash
codex mcp login corply
```

After authentication, retry the blocked read once. If the active process still does not see the
connection, explain that a fresh agent session is required; do not restart the company workflow or
create duplicate state.
