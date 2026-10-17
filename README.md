# MoDineX plugin for Claude

[MoDineX](https://mogenix.de) is a restaurant point-of-sale and back-office system by MoGeniX. This plugin connects Claude to a MoDineX account through the hosted MCP server at `https://mogenix.de/api/mcp` and adds skills for everyday restaurant questions.

## Install

```
/plugin install mogenix --marketplace bioma-coder/modinex-claude-plugin
```

Then run `/mcp`, choose `mogenix` and sign in. The MoDineX consent page lets you pick the organization, branches and data to share. An existing MoDineX account is required.

## What Claude can do

- Sales summaries and breakdowns by day, hour, payment method or menu item
- Menu lookup and review in English, German and Arabic
- Stock levels, reorder needs and supplier invoices
- VAT overview and payroll totals (overview only, not tax advice; no per-employee data)
- Online-shop and delivery-platform orders (no customer data)
- Menu-change drafts (name, description or price). Drafts never change the live menu; the owner approves them inside MoDineX.

## Privacy and support

- Privacy policy: https://mogenix.de/privacy
- Terms: https://mogenix.de/terms
- Support: support@mogenix.de · https://mogenix.de/support

Revoke access at any time in MoDineX under Settings > External AI Connections.

## License

MIT, see [LICENSE](LICENSE).
