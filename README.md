# mcp-weather
play around with model context protocol
docu: https://modelcontextprotocol.io/quickstart/server

## set up env
curl -LsSf https://astral.sh/uv/install.sh | sh

# Create a new directory for our project
uv init weather
cd weather

# Create virtual environment and activate it
uv venv
source env_MCP/bin/activate

# Install dependencies
uv add "mcp[cli]" httpx

# Create our server file
touch weather.py