# File Naming Conventions

This vault uses structured naming to support search-ability, link-ability, and semantic categorisation.

## System Folders (`/system/`)

Format:  
`[pv-tag]-[focus-area]-[short-title].md`

Example:  
`pv3.6-modulation-smoothing.md`

### Multiple PV Tags

Use the primary PV tag in the filename, and include all associated tags in the front matter.

Example:

Filename:
`pv3.6-modulation-smoothing.md`

Front matter:
```yaml
pv_tags:
  - pv3.6
  - pv1.7
  - pv3.5
```

## Notes

Notebook (raw)  
`YYYY-MM-DD-note-title.md`  
Example: `2025-05-03-blue-phase-questions.md`

Edited Notes  
`[concept]-[slug].md`  
Example: `relevance-field-drift-capture.md`

## Research

External papers:  
`[author-year]-[short-title].md`  
Example: `chalmers-1996-conscious-mind.md`

## Engineering

Modules  
`[ucse-tag]-[component]-[function].md`  
Example: `ucse1.2-scaffold-operator.md`

Scripts  
`[tool]-[action].sh` or `.rs`, etc.  
Example: `sync-vault.sh`, `generate-diagram.rs`

## Notes

- Avoid spaces; use `-` for separation
- Use lowercase to reduce conflicts across systems
- Use consistent tag or prefix formats for filtering in Obsidian