# Steps to install MCPs

**NOTE** - Some of these MCPs need your Github Personal Access Token and other API Keys so create them and be ready & also login to Smithery.ai with your Github

## 1. Smithery Github - https://smithery.ai/server/@smithery-ai/github

1. Go to the above link, and in the installation section - Select Cursor

2. Paste your Github PAT and "Save and Connect"

3. Copy the provided MCP JSON into your mcp.json file in Cursor

## 2. Firecrawl - https://smithery.ai/server/@mendableai/mcp-server-firecrawl

1. Go to the above link, and in the installation section - Select Cursor

2. Paste your FireCrawl API Key and "Save and Connect"

3. Copy the provided MCP JSON into your mcp.json file in Cursor

## 3. Sequential Thinking - https://smithery.ai/server/@smithery-ai/server-sequential-thinking

1. Go to the above link, and in the installation section - Select Cursor

2. Copy the provided MCP JSON into your mcp.json file in Cursor

## 4. BrowserTools AgentDesk - https://browsertools.agentdesk.ai/installation

1. From the above link, follow steps 1 & 2 of Downloading BrowserTools Chrome extension and Install it in your Google Chrome Extensions Manager.

2. Now we have to generate the MCP JSON part for this extension with your local paths.

3. Run this command to get your NODE_PATH and copy it -

```bash
which node
```

4. Run the BrowserTools Agent Command using npx

```bash
npx @agentdeskai/browser-tools-mcp@1.2.0
```

5. In a separate terminal run BrowserTools Server Command using npx

```bash
npx @agentdeskai/browser-tools-server@1.2.0
```

6. In another terminal run this command to get your MCP_SERVER_PATH and copy it-

```bash
find ~/.npm/_npx -name "browser-tools-mcp" -type d
```

7. Now add both copied paths in the below format and add this JSON to your mcp.json file in Cursor

"browser-tools": {
      "command": "NODE_PATH",
      "args": [
        "MCP_SERVER_PATH",
        "run"
      ],
      "enabled": true
    }

8. Keep in mind you have to keep running both Step 4 & Step 5 terminals while using cursor to keep the connection alive.

9. In your browser you will now see an "BrowserToolsMCP" tab in DevTools. 

10. Open it and add **Screenshot Settings** - set path where to save the screenshots.