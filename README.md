# Veval Docs

Source for the Veval documentation site.

## Local development

Install the CLI:

```bash
npm i -g mint
```

Run the dev server from the repo root:

```bash
mint dev
```

Preview at `http://localhost:3000`.

## Publishing

Changes pushed to the default branch deploy automatically.

## Troubleshooting

- Dev server won't start: run `mint update` to get the latest CLI version
- Page shows 404: confirm the page is listed in `docs.json` under `navigation`
