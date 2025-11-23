---
title: Authoring Content
---

Quartz supports **Obsidian-flavored Markdown**. This means you can write content almost exactly how you would in Obsidian.

## File Structure

Quartz uses a file structure similar to Obsidian:

```
content/
├── index.md
├── notes/
│   ├── note1.md
│   └── note2.md
└── assets/
    ├── image1.png
    └── image2.jpg
```

## Frontmatter

You can add metadata to your notes using YAML frontmatter:

```yaml
---
title: My Note Title
description: A brief description of the note
tags: [tag1, tag2]
date: 2024-01-01
---
```

## Links and Embeds

Quartz supports:
- **Wikilinks**: `[[Note Title]]` or `[[Note Title|Display Text]]`
- **Markdown links**: `[Display Text](path/to/note.md)`
- **Transclusions**: `![[Note Title]]` to embed content from other notes
- **Images**: `![Alt text](path/to/image.png)`

## Features

- **Full-text search** across all your content
- **Graph view** to visualize connections between notes
- **Backlinks** to see what references each note
- **Table of contents** automatically generated
- **Syntax highlighting** for code blocks
- **LaTeX math** support
- **Popover previews** when hovering over links
