# Vibe Prospecting

<img src="logo.png" alt="Vibe Prospecting Logo" width="90">

**Power your chat with live B2B data — build lead lists, research companies, enrich contacts, and personalize outreach, all from inside your AI assistant.**

Vibe Prospecting is a **remote MCP server**. There's nothing to run locally and no API key to manage — you connect over a single URL and sign in through your browser on first use.

> **MCP endpoint:** `https://vibeprospecting.explorium.ai/mcp`

---

## What you can do

- 🔎 **Find companies** by name, domain, industry, size, location, tech stack, and more
- 👤 **Discover & enrich contacts** — roles, profiles, and buying signals at any company
- 🏢 **Research firms** — firmographics, technographics, funding, competitors, and challenges
- 📈 **Analyze & export** — preview a sample instantly, then export the full dataset to CSV when you're ready

You always see a **sample preview first** (5–10 rows). The full dataset is only processed when you explicitly ask to export — so exploring is fast and credit-friendly.

---

## Installation

Pick your tool below. All clients connect to the same remote endpoint and authenticate through your browser (OAuth) on first use.

### Claude Code  ⭐ recommended

One line — paste it into your terminal:

```bash
claude mcp add --transport http vibe-prospecting https://vibeprospecting.explorium.ai/mcp
```

Then start (or restart) Claude Code and run a prompt that uses it (see [Examples](#examples)). The first call opens your browser to sign in. Verify the connection anytime with:

```bash
claude mcp list
# vibe-prospecting: https://vibeprospecting.explorium.ai/mcp - ✓ Connected
```

### Cowork & Claude Desktop

Add it as a custom connector through the UI (no terminal needed):

1. Open **Customize → Connectors** in Chat/Cowork/Code in Claude Desktop 
2. Click the **+** next to *Connectors* and choose **Browse connectors**
3. Under `Anthropic & Partners` look for **Name:** `Vibe Prospecting` — **URL:** `https://vibeprospecting.explorium.ai/mcp`
4. Click **+** and then click **Install**, then follow the sign-in prompts to grant access

Once added, Vibe Prospecting's tools are available to Claude automatically.

### Codex CLI

One command — Codex detects OAuth automatically and opens your browser to sign in:

```bash
codex mcp add vibe-prospecting --url https://vibeprospecting.explorium.ai/mcp
```

Confirm it's connected with `codex mcp list` (look for `Auth: OAuth`), or start a Codex session and run `/mcp` to see its tools. If you ever need to re-authenticate, run `codex mcp login vibe-prospecting`.

> **No native OAuth in your Codex version?** Use the universal `mcp-remote` bridge instead. Add this block to `~/.codex/config.toml` — it opens the browser for sign-in on first use:
>
> ```toml
> [mcp_servers.vibe-prospecting]
> command = "npx"
> args = ["-y", "mcp-remote", "https://vibeprospecting.explorium.ai/mcp"]
> ```

### Gemini CLI

Install the extension directly from this repository:

```bash
gemini extensions install https://github.com/explorium-ai/vibeprospecting-mcp
```

The extension is loaded and managed automatically by Gemini CLI, and OAuth sign-in is handled on first use. See the [Gemini CLI extensions docs](https://geminicli.com/docs/extensions/) for details.

---

## Examples

Once connected, just ask in plain language:

```
Who should I contact for a partnership with monday.com? Get anyone who can
promote a partnership with them, with all the contact details you can find.
```

```
What are the business challenges of Amazon?
```

```
Get the engineering leadership team at Palo Alto Networks.
```

```
Find B2B SaaS companies in New York with 50–200 employees, then enrich
the decision-makers and export the list to CSV.
```

---

## Authentication & credits

- **Sign-in:** OAuth through your browser on first use — no API keys to copy or store.
- **Free to explore:** searching and previewing samples is lightweight. Exporting the full dataset uses credits.
- **Pricing & credits:** <https://www.vibeprospecting.ai/pricing>

---

## Troubleshooting

- **`Failed to connect` / error `-32000` in Claude Code** — this happens with the old local `uvx vibeprospecting-mcp` (stdio) command. That path is **deprecated**; use the `--transport http` command above instead.
- **Connector won't connect in Cowork/Desktop** — the server is reached from Anthropic's cloud, so the URL must be publicly reachable. Double-check the URL is exactly `https://vibeprospecting.explorium.ai/mcp`.
- **Re-authenticate** — in Claude Code run `claude mcp remove vibe-prospecting` then re-add it; in Codex run `codex mcp login vibe-prospecting` again.

---

## Support & documentation

- [API Documentation](https://docs.vibeprospecting.ai)
- [Support & Help Center](https://www.vibeprospecting.ai/contact-us)
- [Vibe Prospecting Homepage](https://www.vibeprospecting.ai)

For technical support, contact support@vibeprospecting.ai.

## License

This project is licensed under the Explorium Term of Service. See [Term of Service](https://www.vibeprospecting.ai/terms-of-service) for details.
