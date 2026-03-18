---
name: shard-doc
description: "Split large markdown documents into smaller, organized files based on level 2 sections."
---

# Shard Document

**Goal:** Split large markdown documents into smaller files using `npx @kayvan/markdown-tree-parser`.

## EXECUTION

### Step 1: Get Source Document
- Ask user for source document path
- Verify file exists and is markdown

### Step 2: Get Destination Folder
- Default: same location, folder named after source file
- Ask user to confirm or provide custom path

### Step 3: Execute Sharding
- Run: `npx @kayvan/markdown-tree-parser explode [source] [destination]`

### Step 4: Verify Output
- Check destination contains sharded files and index.md

### Step 5: Report Completion
- Display summary with file counts

### Step 6: Handle Original Document
- Options: [d] Delete, [m] Move to archive, [k] Keep (not recommended)
