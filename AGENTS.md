# Institutional AI Knowledge Handbook — Agent Instructions

## About This Repo

This is a curated personal knowledge base capturing research, reports, and notes on **institutional AI**: how organisations design, govern, operate, and scale AI systems — with a focus on DS/ML teams and engineering organisations.

Content grows incrementally. Each document is a research dossier covering a specific theme within the space.

## Navigation

Do not load all documents into context. Use the index to identify which documents are relevant to the current conversation.

**Start here:** [`documents/index.md`](documents/index.md)

The index lists every document in the `documents/` folder with its theme, a one-line description, and the key topics it covers. Load only the documents relevant to the user's question.

---

## How to Work

### Answering questions

1. Read `documents/index.md` to understand what documents exist.
2. Identify which documents are relevant based on their themes and topics.
3. Load only those documents into context.
4. If a question spans multiple documents, load each relevant one individually.

### When a new document is added to `documents/`

Update `documents/index.md` to include the new entry. Each entry must follow this format:

```
### [Title](filename.md)
- **Theme:** <value of the `theme` frontmatter field>
- **Description:** <one sentence summary of what the document covers>
- **Key topics:** <comma-separated list of main topics>
```

Read the frontmatter and executive summary of the new file to extract these fields accurately. Do not load the full document to write the index entry.

### When a document is removed

Remove its entry from `documents/index.md`.

### When a document's frontmatter or scope changes

Update its entry in `documents/index.md` to reflect the new theme, description, or topics.
