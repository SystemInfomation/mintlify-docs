# Pals Club Support Portal

A production-quality support documentation site built with [Mintlify](https://mintlify.com), designed to reduce support tickets and guide users to solutions fast.

## Information architecture

| Section | Description |
|---------|-------------|
| **Support Hub** | Landing page, FAQ, and glossary |
| **Getting Started** | Quickstart guide and system requirements |
| **Account & Billing** | Account management, subscriptions, and account recovery |
| **Using Pals Club** | Features overview and core workflow guides |
| **Troubleshooting** | Common issues, decision-tree playbook, and diagnostics collection |
| **Status & Incidents** | Platform status and incident process |
| **Safety & Legal** | Community guidelines, privacy controls, terms, and privacy policy |
| **Developers** | API overview and integration placeholders |
| **Contact Support** | Support channels, escalation guide, and request templates |

## Development

Install the [Mintlify CLI](https://www.npmjs.com/package/mint) to preview the documentation locally:

```bash
npm i -g mint
```

Run the development server at the root of this repository (where `docs.json` is located):

```bash
mint dev
```

View your local preview at `http://localhost:3000`.

## Deployment

### Option A: Mintlify hosting (recommended)

1. Install the [Mintlify GitHub app](https://dashboard.mintlify.com/settings/organization/github-app) from your dashboard.
2. Push changes to the default branch — deployments happen automatically.

### Option B: Self-hosted (Vercel / Netlify / GitHub Pages)

Mintlify generates static output that can be deployed to any static hosting provider. Refer to the [Mintlify deployment docs](https://mintlify.com/docs/quickstart) for details.

## Extending the docs

- **Add a new page**: Create an MDX file in the appropriate directory and add its path to `docs.json` under the correct navigation group.
- **Update navigation**: Edit the `navigation.tabs` array in `docs.json`.
- **Check for broken links**: Run `mint broken-links` locally.
- **Validate changes**: Run `mint dev` and review pages in the browser before pushing.

## Placeholders

This documentation uses placeholder values (e.g., `[CONTACT_EMAIL]`, `[STATUS_PAGE_URL]`, `[BILLING_PROVIDER]`) where product-specific details are needed. Search for `[` across MDX files to find and replace all placeholders with real values.

## Resources

- [Mintlify documentation](https://mintlify.com/docs)
- [MDX syntax reference](https://mintlify.com/docs/text)
- [Component reference](https://mintlify.com/docs/components)
