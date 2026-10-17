# MoDineX plugin for Claude

MoDineX is the restaurant POS by MoGeniX. This plugin connects Claude Code to a
MoDineX account through the hosted MCP server at `https://mogenix.de/api/mcp`
and adds six skills:

- sales review (`mogenix-sales-review`)
- menu review (`mogenix-menu-review`)
- menu-change drafts (`mogenix-menu-change-draft`)
- stock & supplier invoices (`mogenix-stock-invoices`)
- VAT & payroll overview (`mogenix-vat-payroll-overview`)
- online orders & sales breakdown (`mogenix-orders-breakdown`)

## Install

```
/plugin install mogenix --marketplace bioma-coder/modinex-claude-plugin
```

Then run `/mcp`, choose `mogenix` and sign in. The browser opens the MoDineX
consent page; pick the branches to share. No client ID or fixed callback port
is needed: Claude Code identifies itself with its standard client metadata
document and any free local port works.

All tools are read-only except `mogenix_prepare_menu_change`, which only creates
private drafts; drafts are approved and executed only in the MoDineX app.
Revoke access in MoDineX under Settings → External AI Connections.

On claude.ai, use the **MoDineX** connector from the Claude Directory.
