# OpenCode + Burp Suite MCP

<p align="center">
  <img src="Connecting%20OpenCode%20to%20Burp%20Suite.png" alt="OpenCode connected to Burp Suite through MCP" width="100%">
</p>

Connect [OpenCode](https://opencode.ai/) to [Burp Suite](https://portswigger.net/burp) using the Model Context Protocol (MCP).

This repository contains the OpenCode configuration used to connect to a locally running Burp Suite MCP server.

## Configuration

The `opencode.json` file in this repository contains:

```json
{
  "$schema": "https://opencode.ai/config.json",
  "mcp": {
    "servers": {
      "burp": {
        "type": "remote",
        "url": "http://127.0.0.1:9876/mcp",
        "oauth": false,
        "disabled": false
      }
    }
  }
}
```

Make sure the Burp Suite MCP server is running and listening at `http://127.0.0.1:9876/mcp` before starting the connection in OpenCode.

## Repository files

- `opencode.json` — OpenCode MCP server configuration.
- `.gitignore` — Common local files and secrets to exclude from Git.
- `LICENSE` — MIT License.

## YouTube

📺 Watch more AI, cybersecurity, and technology experiments on [ULTIMAX](https://www.youtube.com/@ultimax-hacks).

## Safety

Only test websites and applications that you own or have explicit permission to assess. Review actions before running them and take care not to expose sensitive information.

---

Made by **ULTIMAX**.
