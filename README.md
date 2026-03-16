# Aionis Docs

This repository contains the standalone Mintlify documentation site for Aionis.

## Structure

- `docs.json`: Mintlify site configuration
- `index.mdx`: homepage
- `why/`, `what/`, `how/`, `reference/`: the current external documentation structure
- `guide/`: legacy compatibility pages kept for older links
- `api-reference/`: API docs
- `operations/`: production operations docs
- `proof/`: proof and applied evidence path

## Deploy to Mintlify

1. Create or open the Mintlify project for this repository.
2. Connect this repository in Mintlify.
3. Keep the docs root at the repository root.
4. Set the custom domain to `doc.aionisos.com` in Mintlify.
5. Add the DNS CNAME record:
   - host: `doc`
   - value: `cname.mintlify-dns.com`
6. Push to the default branch to trigger deployment.

## Local preview

```bash
npm i -g mint
mint dev
```

## Validation

```bash
mint validate
```
