# Vibe Prospecting MCP

<img src="https://raw.githubusercontent.com/explorium-ai/vibeprospecting-mcp/main/logo.png" alt="Vibe Prospecting Logo" width="90">

**Power your chat with B2B data to create lead lists, research companies, personalize your outreach, and more.**

[![Version](https://img.shields.io/github/package-json/v/explorium-ai/vibeprospecting-mcp?style=flat-square&color=blue)](https://github.com/explorium-ai/vibeprospecting-mcp) [![Downloads](https://img.shields.io/badge/downloads-150k%2B-22c55e?style=flat-square&logo=npm&logoColor=white)](https://www.npmjs.com/package/@vibeprospecting/vpai) [![MCP](https://img.shields.io/badge/MCP-server-0052CC?style=flat-square)](https://modelcontextprotocol.io) [![Claude](https://img.shields.io/badge/Claude-compatible-7C3AED?style=flat-square&logo=anthropic&logoColor=white)](https://claude.ai) [![ChatGPT](https://img.shields.io/badge/ChatGPT-compatible-74AA9C?style=flat-square&logo=openai&logoColor=white)](https://chatgpt.com) [![Gemini CLI](https://img.shields.io/badge/Gemini_CLI-extension-4285F4?style=flat-square&logo=google&logoColor=white)](https://geminicli.com) [![GitHub Stars](https://img.shields.io/github/stars/explorium-ai/vibeprospecting-mcp?style=flat-square&logo=github)](https://github.com/explorium-ai/vibeprospecting-mcp) [![MIT License](https://img.shields.io/badge/license-MIT-blue?style=flat-square)](LICENSE)

[Overview](#overview) · [Installation](#installation) · [Use Cases](#use-cases) · [Examples](#examples) · [Usage](#usage) · [Support](#support)

---

## Overview

Vibe Prospecting MCP is an MCP server that gives AI assistants live access to comprehensive company and contact data. It provides business intelligence, enrichment, and workflow automation capabilities natively inside Claude, ChatGPT, and Gemini CLI.

- **Company Search**: Find companies by name, domain, industry, size, location, or tech stack
- **Contact Discovery**: Locate and enrich business contacts with verified emails and profiles
- **Real-Time Data**: Access up-to-date business information from 150M+ companies and 800M+ professionals
- **Seamless Integration**: Works natively with Claude CoWork, ChatGPT, and Gemini CLI

## Features

- Search and retrieve company profiles and firmographics
- Discover and enrich contact information
- Scale up to 1,000 companies or contacts in a single query. For larger workloads, use the [Vibe Prospecting Plugin](https://github.com/explorium-ai/vibeprospecting-plugin)
- Preview sample results instantly before committing to a full export
- See credit cost upfront before exporting
- Chain workflows across companies and contacts (cross-entity prospecting)
- Export structured results as CSV
- Secure, real-time access via MCP protocol

---

## Installation

### Claude CoWork

Vibe Prospecting is available natively in **Claude CoWork** - no installation required. Connect it from your CoWork settings and start prospecting immediately.

For Claude Code, use the [Vibe Prospecting Plugin](https://github.com/explorium-ai/vibeprospecting-plugin) instead.

### Gemini CLI

Install the extension directly from this repository:

```bash
gemini extensions install https://github.com/explorium-ai/vibeprospecting-mcp
```

Or link a local clone for development:

```bash
gemini extensions link /path/to/vibeprospecting-mcp
```

OAuth authentication is handled automatically on first use. No API key required.

---

## Use Cases

**Use Case** &nbsp; `Build Lead Lists` &nbsp; `Find Contact Info` &nbsp; `Account Research` &nbsp; `Personalize Outreach` &nbsp; `Meeting Prep` &nbsp; `Recruiting`

**Best for** &nbsp; `Founders` &nbsp; `Sales` &nbsp; `Recruiters` &nbsp; `Marketers`

---

## Examples

Browse the full [Prompt Library](https://www.vibeprospecting.ai/prompt-library) for ready-to-use prompts.

### Build Lead Lists

```
Find marketing decision makers at small digital agencies (1-50 employees)
in Texas and Florida whose websites mention advertising services.
Include contact details where available.
```

### Find Contact Info

```
Find data decision makers at companies with 100-1,000 employees that use
Snowflake. Return only verified emails.
```

### Account Research

```
Give me a full overview of Stripe: what they do, their competitive
landscape, key business challenges, and main pain points.
```

### Personalize Your Outreach

```
Write a personalized outreach message to the Head of Marketing at Intuit.
Use recent company signals to make it relevant and maximize reply rates.
```

### Meeting Prep

```
Who should I contact for a partnership with monday.com?
Get anyone who can promote a partnership with them, bring me all the
contact details you can find.
```

### Recruiting

```
Find DevOps or platform engineers in Texas at mid-market information
security companies with 18+ months in their current role.
```

---

## Usage

### Claude CoWork

- Connect Vibe Prospecting from your CoWork settings
- Start prompting in natural language - no setup required
- Schedule and trigger prospecting tasks directly from CoWork

### Gemini CLI

- The extension is automatically loaded and managed by Gemini CLI
- OAuth authentication is handled automatically on first use
- For more information, see the [Gemini CLI documentation](https://geminicli.com/docs/extensions/)

---

## Support

- [Vibe Prospecting Homepage](https://www.vibeprospecting.ai)
- [API Documentation](https://developers.explorium.ai/mcp-docs/vibeprospecting)
- [Prompt Library](https://www.vibeprospecting.ai/prompt-library)
- [YouTube](https://www.youtube.com/@VibeProspecting)
- [Support & Help Center](https://www.vibeprospecting.ai/contact-us)

For technical support, contact support@vibeprospecting.ai.

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
