uv init
uv venv
source .venv/bin/activate
uv add "mcp[cli]"

uv run mcp-server