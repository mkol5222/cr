# CR - my container registry

## Images:

### openroute-mcp

Build source: [openroute-mcp/Dockerfile](openroute-mcp/Dockerfile)

This repo includes a manual GitHub Actions workflow that publishes a single mutable image tag to GitHub Container Registry:

`ghcr.io/<your-github-user-or-org>/openroute-mcp:latest`

To publish it:

1. Push this repository to GitHub.
2. Open the `Actions` tab.
3. Run the `Publish openroute-mcp image` workflow manually.
4. If this is the first push, open the package in GHCR and set visibility to `Public` if GitHub did not inherit that automatically.

To pull it later:

```sh
docker pull ghcr.io/<your-github-user-or-org>/openroute-mcp:latest
```

To run it:

```sh
docker run --rm ghcr.io/<your-github-user-or-org>/openroute-mcp:latest
```

If the package is public, no login is required for pull. If it stays private, login first:

```sh
echo "$GITHUB_TOKEN" | docker login ghcr.io -u <your-github-user-or-org> --password-stdin
```

### sparfenyuk-mcp-proxy-with-npx_uv

Build source: [quantum-management-mcp/Dockerfile](quantum-management-mcp/Dockerfile)

This repo also includes a manual GitHub Actions workflow for publishing a single mutable tag to GitHub Container Registry:

`ghcr.io/<your-github-user-or-org>/sparfenyuk-mcp-proxy-with-npx_uv:latest`

To publish it:

1. Push this repository to GitHub.
2. Open the `Actions` tab.
3. Run the `Publish sparfenyuk-mcp-proxy-with-npx_uv image` workflow manually.
4. If this is the first push, open the package in GHCR and set visibility to `Public` if GitHub did not inherit that automatically.

To pull it later:

```sh
docker pull ghcr.io/<your-github-user-or-org>/sparfenyuk-mcp-proxy-with-npx_uv:latest
```

To run it:

```sh
docker run --rm ghcr.io/<your-github-user-or-org>/sparfenyuk-mcp-proxy-with-npx_uv:latest
```


