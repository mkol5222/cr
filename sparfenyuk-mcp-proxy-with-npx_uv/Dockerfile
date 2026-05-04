FROM ghcr.io/sparfenyuk/mcp-proxy:latest

# add Python
# Install the 'uv' package
RUN python3 -m ensurepip && pip install --no-cache-dir uv

ENV PATH="/usr/local/bin:$PATH" \
    UV_PYTHON_PREFERENCE=only-system

# add NodeJS
RUN apk add npm nodejs

ENTRYPOINT ["catatonit", "--", "mcp-proxy"]