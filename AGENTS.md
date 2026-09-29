# Documentation project instructions

## About this project

- Veval documentation site
- Pages are MDX files with YAML frontmatter
- Configuration lives in `docs.json`
- Run `mint dev` to preview locally
- Run `mint broken-links` to check links

## Structure

- `concepts/` pages explain what something is: a one-line definition, "How X fits in", reference tables, and "Deep dives" cards. No long code samples.
- `guides/` pages and `quickstart.mdx` show how to do something, with code in all three languages. End each with "What's next" cards.
- `llm-reference.mdx` is the single-page SDK reference, also used as AI context.
- No `---` rules between sections. Use `<Steps>` for sequential instructions.

## Terminology

- **Trace** — a recorded agent run (input, output, steps, cost, timing)
- **Step** — a single LLM call or sub-operation within a trace
- **Scenario** — a named set of test items run against your agent
- **Snapshot** — a stored known-good run (every step with its input and output), used to detect changed prompts/tool arguments and added, removed, or reordered steps
- **Replay** — running an agent against a recorded trace with mocked LLM responses

## Style preferences

- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references
- All code examples must include C#, Python, and Node variants
