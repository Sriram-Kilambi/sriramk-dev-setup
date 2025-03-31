# MCP Servers List

From Smithery MCP website install the following MCP Servers for Cursor

```json
{
  "mcpServers": {
    "@smithery-ai-github": {
      "command": "npx",
      "args": [
        "-y",
        "@smithery/cli@latest",
        "run",
        "@smithery-ai/github",
        "--config",
        "{\"githubPersonalAccessToken\":\"GITHUB_PERSONAL_ACCESS_TOKEN\"}"
      ]
    },
    "@mendableai-mcp-server-firecrawl": {
      "command": "npx",
      "args": [
        "-y",
        "@smithery/cli@latest",
        "run",
        "@mendableai/mcp-server-firecrawl",
        "--config",
        "{\"fireCrawlApiKey\":\"FIRECRAWL_KEY\"}"
      ]
    },
    "@smithery-ai-server-sequential-thinking": {
      "command": "npx",
      "args": [
        "-y",
        "@smithery/cli@latest",
        "run",
        "@smithery-ai/server-sequential-thinking",
        "--config",
        "{}"
      ]
    },
    "browser-tools": {
      "command": "/Users/sriramkilambi/.nvm/versions/node/v20.18.1/bin/node",
      "args": [
        "/Users/sriramkilambi/.npm/_npx/dcd6f0de5842aab6/node_modules/@agentdeskai/browser-tools-mcp/dist/mcp-server.js",
        "run"
      ],
      "enabled": true
    }
  }
}
```

### Commands for each of these servers are as follows - These will be set an alias in .zshrc for easy access.

@smithery-ai-github -

npx -y @smithery/cli@latest run @smithery-ai/github --config "{\"githubPersonalAccessToken\":\"GITHUB_PERSONAL_ACCESS_TOKEN\"}"

@mendableai-mcp-server-firecrawl -

npx -y @smithery/cli@latest run @mendableai/mcp-server-firecrawl --config "{\"fireCrawlApiKey\":\"FIRECRAWL_KEY\"}"

@smithery-ai-server-sequential-thinking -

npx -y @smithery/cli@latest run @smithery-ai/server-sequential-thinking --config "{}"

browser-tools -

npx @agentdeskai/browser-tools-server@1.2.0

npx @agentdeskai/browser-tools-mcp@1.2.0

## NOTE - ALWAYS RUN BROWSER TOOLS SERVER BEFORE RUNNING BROWSER TOOLS AGENT SO THAT THE AGENT CAN CONNECT TO THE SERVER.
