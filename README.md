# Kanbix

Manage your Kanbix work from ChatGPT, Codex or Claude: find cards, review priorities and organize tasks and their relationships in the board you authorize.

This package is prepared for public distribution. It is not a published directory listing yet.

## Connect

1. Install the Kanbix plugin in your assistant, or add the remote MCP endpoint `https://api.kanbix.com.br/mcp` for a development test.
2. Use OAuth with automatic client registration (DCR). Sign in on Kanbix, choose your board and review permissions. No shared API key or fixed board header is needed.
3. Start with reading your board. To create or edit tasks, authorize the corresponding write permissions in Kanbix.

The account must have a verified email and access to the selected board. Board policies and account limits continue to apply. Available tools depend on the permissions you grant. One grant is associated with a user and OAuth client; reconnecting that pair to a different board revokes its previous grant. Revoke access from Kanbix's authorized-connections settings.

A Codex local MCP entry is independent from a ChatGPT or Claude connection. Connect separately in each host. Never paste passwords, access tokens or verification codes into chat.

## Package contents

- `plugin.json` and `mcp.json`: portable Agent Plugins package, with OpenAI presentation metadata and OAuth DCR discovery.
- `.claude-plugin/plugin.json` and `.mcp.json`: Claude-compatible metadata and remote HTTP MCP connection.
- `skills/manage-kanbix/SKILL.md`: Kanbix task workflow shared by the supported hosts.
- `assets/`: Kanbix brand assets.

The package contains no tenant IDs, credentials, backend source code or local shell hooks. OAuth uses the remote Kanbix service, so a working Kanbix account and network connection are required. These capabilities remain subject to each host's current support and directory review.

## Support and policies

- Website: https://www.kanbix.com.br
- Support: https://www.kanbix.com.br/contato — contato@kanbix.com.br
- Privacy: https://www.kanbix.com.br/privacy
- Terms: https://www.kanbix.com.br/terms

The integration package is licensed under the MIT License; see LICENSE. This license covers the package distributed in this repository. The separately hosted Kanbix application, backend, infrastructure, customer data and credentials are not included and are not licensed by this package. No trademark rights to the Kanbix name or brand are granted.

Source: https://github.com/GabDevjs/kanbix-plugin

Public directory listings remain subject to OpenAI and Anthropic review. A public GitHub repository is not itself a directory approval.
