# Claude Code Plugins Directory

A curated directory of high-quality plugins for Claude Code.

> **Note:** Make sure you trust a plugin before installing, updating, or using it. Review each plugin's source code and documentation before use.

## Available Plugins

| Provider | MCP Server | Description |
|----------|------------|-------------|
| AWS | [aws-knowledge-mcp-server](./plugins/aws-knowledge-mcp-server) | Access up-to-date AWS documentation, code samples, API references, and regional availability data |
| AWS | [aws-diagram-mcp-server](./plugins/aws-diagram-mcp-server) | Create AWS architecture diagrams, sequence diagrams, flow charts, and class diagrams using Python diagrams DSL |
| AWS | [aws-pricing-mcp-server](./plugins/aws-pricing-mcp-server) | Get real-time AWS pricing data, cost analysis, and optimization recommendations using natural language queries |
| AWS | [aws-api-mcp-server](./plugins/aws-api-mcp-server) | Execute and suggest AWS CLI commands with validation, security controls, and hallucination protection |
| AWS | [amazon-bedrock-agentcore-mcp-server](./plugins/amazon-bedrock-agentcore-mcp-server) | Search and access Amazon Bedrock AgentCore documentation, APIs, tutorials, and best practices |
| AWS | [terraform-mcp-server](./plugins/terraform-mcp-server) | Terraform development on AWS with best practices, security scanning via Checkov, and AWS provider documentation |
| AWS | [cdk-mcp-server](./plugins/cdk-mcp-server) | AWS CDK best practices, AWS Solutions Constructs, GenAI CDK patterns, and CDK Nag security validation |
| Tavily | [tavily-mcp-server](./plugins/tavily-mcp-server) | Real-time web search and intelligent content extraction powered by Tavily |

## Installation

Plugins can be installed directly from this marketplace via Claude Code's plugin system.

To install, run `/plugin install {plugin-name}@dminhk/claude-plugins`

or browse for the plugin in `/plugin > Discover`

## Prerequisites

Most plugins require specific dependencies:

- **AWS MCP Servers**: `uv` package manager, Python 3.10+
- **aws-diagram-mcp-server**: GraphViz
- **aws-pricing-mcp-server**: AWS credentials with `pricing:*` permissions
- **aws-api-mcp-server**: AWS CLI and credentials
- **terraform-mcp-server**: Terraform CLI, Checkov
- **cdk-mcp-server**: AWS CDK CLI (`npm install -g aws-cdk`)
- **tavily-mcp-server**: `TAVILY_API_KEY` environment variable

## Plugin Structure

Each plugin follows a standard structure:

```
plugin-name/
├── .claude-plugin/
│   └── plugin.json      # Plugin metadata (required)
├── .mcp.json            # MCP server configuration (optional)
├── commands/            # Slash commands (optional)
├── agents/              # Agent definitions (optional)
├── skills/              # Skill definitions (optional)
└── README.md            # Documentation
```

## Contributing

To suggest a plugin for inclusion, please open an issue or submit a pull request.

## Documentation

For more information on developing Claude Code plugins, see the [official documentation](https://docs.anthropic.com/en/docs/claude-code).
