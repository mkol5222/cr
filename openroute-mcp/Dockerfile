FROM python:3.12-slim
WORKDIR /app
RUN pip install uv
RUN uv pip install --system openroute-mcp
CMD ["openroute-mcp"]