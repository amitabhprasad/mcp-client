uv init
uv venv
source .venv/bin/activate
uv add "mcp[cli]"

uv run mcp-server

# Since pyproject.toml is inside subdir...use this command
uvx --from "git+https://github.com/amitabhprasad/mcp-client.git#subdirectory=mcp-server-deepdive-deployment" mcp-server

```json
{
    "mcpServers"{
      "add_tool": {
      "command": "uvx",
      "args": [
        "--from",
        "git+https://github.com/amitabhprasad/mcp-client.git#subdirectory=mcp-server-deepdive-deployment",
        "mcp-server"
      ]
    }
  }
}
```
