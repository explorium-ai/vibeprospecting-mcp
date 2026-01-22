# Vibe Prospecting

<img src="logo.png" alt="VibeProspecting Logo" width="90">

**Power your chat with B2B data to create lead lists, research companies, personalize your outreach, and more.**

## Overview

Vibe Prospecting is an MCP server that enables access to live, comprehensive company and contact data. It provides seamless business intelligence, enrichment, and workflow automation capabilities for AI tools like Gemini CLI.

- **Company Search**: Find companies by name, domain, or attributes.
- **Contact Discovery**: Locate and enrich business contacts.
- **Real-Time Data**: Access up-to-date business information.
- **Seamless Integration**: Works natively with Gemini CLI.

## Features

- Search and retrieve company profiles and firmographics
- Discover and enrich contact information
- Integrate Vibe Prospecting data into AI workflows
- Secure, real-time access via MCP protocol

## Examples

### Example 1: Partnership Opportunity Research

```
Who should I contact for partnership with monday.com? Get anyone who can promote a partnership with them. Bring me all the contact details you can find
```

### Example 2: Business Challenge Analysis

```
What are the business challenges of amazon?
```

### Example 3: Leadership Team Discovery

```
Get the engineering leadership team at Palo Alto Networks
```

## Installation

### Gemini CLI

Install the extension directly from this repository:

```bash
gemini extensions install https://github.com/explorium-ai/mcp-explorium
```

Or for development:

```bash
gemini extensions link /path/to/mcp-explorium
```

### Docker Deployment

For self-hosting with Docker:

```bash
docker build -t vibe-prospecting-mcp .
docker run -e API_ACCESS_TOKEN=your_token vibe-prospecting-mcp
```

**Required**: `API_ACCESS_TOKEN` environment variable for authentication.

## Usage

### Gemini CLI

- The extension is automatically loaded and managed by Gemini CLI
- OAuth authentication is handled automatically on first use
- For more information, refer to the [Gemini CLI documentation](https://geminicli.com/docs/extensions/)

### Docker

- Requires API access token for authentication
- Server runs on port 44280 by default
- Connect via MCP remote protocol

## Support & Documentation

- [API Documentation](https://developers.explorium.ai/mcp-docs/vibeprospecting)
- [Support & Help Center](https://www.vibeprospecting.ai/contact-us)
- [Vibe Prospecting Homepage](https://www.vibeprospecting.ai)

For technical support, contact support@vibeprospecting.ai.

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.