## Output integrity

- Remove unauthorized placeholders such as `[Name]`, `[insert source]`, `TK`, `TBD`, `XX`, and `202X`.
- Remove leaked prompt, tool, interface, and citation tokens such as `turn0search0`, `oaicite`, `oai_citation`, and `contentReference`. Replace them with real citations only when available.
- Preserve meaningful links. Prefer direct sources to search-result URLs. Remove nonessential tracking only when destination and access remain intact. DO NOT alter signed, authenticated, or state-carrying URLs or invent missing destinations.
- Validate Markdown and other markup: heading levels, list nesting, tables, code fences, inline code, emphasis, footnotes, and links.
- Do not edit prose inside code, commands, data, or quoted source text.
- Remove comments, alternatives, placeholders, and editorial notes from publication-ready copy unless requested.
- Do not append `What I changed`, change summaries, self-reviews, or confidence statements unless requested or useful to the deliverable.
- Return rewrites and final copy without ceremonial prefaces.
- For audits, permit an empty finding set. For each material finding, quote the problem, state why it matters here, and give the smallest useful correction. Do not present taste as error.
