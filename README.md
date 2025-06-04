# bio-mcp-servers
<p>
  <img src="logos/kleon-logo.png" width="100" /> 
  <img src="https://upload.wikimedia.org/wikipedia/commons/5/54/PubMed_logo_blue.svg" width="200"/>
  <img src="https://www.biorxiv.org/sites/default/files/biorxiv_logo_homepage.png" width = "200" />
  <img src="https://biomcp.org/assets/logo.png" width ="200" />
</p>
A compilation for all the available bio agents and a guide to how to use them.

-----------------------------
Quick Start: Claude Desktop Setup¶
The fastest way to get started with BioMCP is to set it up with Claude Desktop:

Install Claude Desktop from Anthropic

Ensure uv is installed:

# Install uv if you don't have it
# MacOS: brew install uv
# Windows: pip install uv
Configure Claude Desktop:

Open Claude Desktop settings

Navigate to Developer section
Click "Edit Config" and add:
{
  "mcpServers": {
    "biomcp": {
      "command": "uv",
      "args": ["run", "--with", "biomcp-python", "biomcp", "run"]
    }
  }
}
Save and restart Claude Desktop
