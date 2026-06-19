# Doitforme Shift for Codex

This private Codex plugin bundles Shift skills and a remote MCP server definition.

## User setup

1. Get your personal `SHIFT_MCP_API_KEY` from the Shift dashboard.
2. Export it in your shell:

```bash
export SHIFT_MCP_API_KEY='<your-key>'
```

3. Install the marketplace and plugin:

```bash
codex plugin marketplace add <path-or-repo-to-distribution/codex-plugin>
codex plugin add doitforme-shift@doitforme-shift-marketplace
```

4. If your Codex installation does not automatically wire the MCP server, add the `doitforme_shift` entry from [`.mcp.json`](./.mcp.json) to your Codex MCP configuration.

## Notes

- API-key auth is static and avoids the OAuth browser flow.
- This plugin keeps using the shared Shift remote MCP backend at `https://backend.shift.doitforme.eu/mcp`.
