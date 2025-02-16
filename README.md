# @harshmaur/mcp-gitlab

[![smithery badge](https://smithery.ai/badge/@harshmaur/gitlab-mcp)](https://smithery.ai/server/@harshmaur/gitlab-mcp)

GitLab MCP(Model Context Protocol) Server.

<a href="https://glama.ai/mcp/servers/7jwbk4r6d7"><img width="380" height="200" src="https://glama.ai/mcp/servers/7jwbk4r6d7/badge" alt="gitlab mcp MCP server" /></a>

## Installation and Execution

### Installing via Smithery

To install GitLab MCP Server for Claude Desktop automatically via [Smithery](https://smithery.ai/server/@harshmaur/gitlab-mcp):

```bash
npx -y @smithery/cli install @harshmaur/gitlab-mcp --client claude
```

### Manual Installation

```bash
npx @harshmaur/mcp-gitlab
```

## Environment Variable Configuration

Before running the server, you need to set the following environment variables:

```bash
GITLAB_PERSONAL_ACCESS_TOKEN=your_gitlab_token
GITLAB_API_URL=your_gitlab_api_url  # Default: https://gitlab.com/api/v4
```

## License

MIT License

## How to use

## Using with Claude App, Cline, Roo Code

When using with the Claude App, you need to set up your API key and URLs directly.

```json
{
  "mcpServers": {
    "GitLab communication server": {
      "command": "npx",
      "args": ["-y", "@harshmaur/mcp-gitlab"],
      "env": {
        "GITLAB_PERSONAL_ACCESS_TOKEN": "your_gitlab_token",
        "GITLAB_API_URL": "your_gitlab_api_url"
      }
    }
  }
}
```

## Using with Cursor

When using with Cursor, you can set up environment variables and run the server as follows:

```bash
env GITLAB_PERSONAL_ACCESS_TOKEN=your_gitlab_token GITLAB_API_URL=your_gitlab_api_url npx @harshmaur/mcp-gitlab
```

- `GITLAB_PERSONAL_ACCESS_TOKEN`: Your GitLab personal access token.
- `GITLAB_API_URL`: Your GitLab API URL. (Default: `https://gitlab.com/api/v4`)
