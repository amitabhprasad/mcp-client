uv init
uv venv
source .venv/bin/activate
uv add "mcp[cli]"
# run server
mcp dev server.py
- this runs the inspector 
# run server as streamable http
uv run server.py