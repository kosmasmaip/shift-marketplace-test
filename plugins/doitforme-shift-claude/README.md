# Doitforme Shift for Claude

This private Claude plugin bundles Shift skills and a remote MCP server definition.

## User setup

1. Get your personal `SHIFT_MCP_API_KEY` from the Shift dashboard.
2. Export it before starting Claude:

```bash
export SHIFT_MCP_API_KEY='<your-key>'
```

3. Add the private marketplace and install the plugin:

```bash
claude plugin marketplace add <path-or-repo-to-distribution/claude-plugin>
claude plugin install doitforme-shift
```

4. If needed, import or merge the MCP configuration from [`.mcp.json`](./.mcp.json) into your project or managed Claude MCP settings.

## Notes

- Claude Code is the recommended Claude client for this plugin.
- Claude Desktop and managed Cowork setups can use the same API key and MCP config, but the distribution flow is usually admin-led.
