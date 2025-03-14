# ~auto~md~

## On-going development & updates via https://github.com/toolworks-dev/auto-md
### (this is just my personal python tool script version in this repo)

-----------------------------------------------------------------------------------------------
### Python tool that converts various file types and GitHub repositories into Markdown documents (.md) optimized for quick RAG/indexing via large language models (LLMs)

Try the web version at https://automd.toolworks.dev

![screen](auto-md-gui-screen.png)

## Features

- Supports multiple file types (see table below)
- Processes zip files/folders/individual files and GitHub repositories
- Generates a single Markdown file or multiple files
- Creates a table of contents and metadata for each file processed

## Supported File Extensions

| Category | Extensions |
|----------|------------|
| Text | .txt, .text, .log |
| Markdown | .md, .markdown, .mdown, .mkdn, .mkd, .mdwn, .mdtxt, .mdtext |
| Web | .html, .htm, .xhtml, .shtml, .css, .scss, .sass, .less |
| Programming | .py, .pyw, .js, .jsx, .ts, .tsx, .java, .c, .cpp, .cs, .go, .rb, .php, .swift, .kt |
| Data | .json, .jsonl, .yaml, .yml, .xml, .csv, .tsv |
| Config | .ini, .cfg, .conf, .config, .toml, .editorconfig |
| Shell | .sh, .bash, .zsh, .fish, .bat, .cmd, .ps1 |
| Other | .rst, .tex, .sql, .r, .lua, .pl, .scala, .clj, .ex, .hs, .ml, .rs, .vim |

## Quick Setup Guide

1. Install Python 3.7 or newer

2. Download this project (or clone repo like normal):
   - Click the green "Code" button above
   - Choose "Download ZIP"
   - Extract the ZIP file

3. Open a terminal/command prompt and navigate to the extracted folder:
   ```
   cd path/to/Auto-MD
   ```

4. Install required packages:
   ```
   pip install -r requirements.txt
   ```

5. Run the application:
   ```
   python main.py
   ```

6. Use the GUI to:
   - Select input files/folders
   - Choose output location
   - Set processing options
   - Click "Start Processing"

## Example Input/Output

### Input

Let's say you have the following files in a folder called "my_project":

- README.md
- script.py
- data.json
- styles.css

### Output

After processing with Auto MD, you would get a single Markdown file (`output.md`) that looks like the example below

This single .md file contains all the content from your input files, with a table of contents at the top for easy navigation and referencing / indexing via LLM models

```markdown
# Auto MD Output

## Table of Contents
- [README](#readme)
- [script](#script)
- [data](#data)
- [styles](#styles)

---

# README

## Metadata
- **Generated on:** 2024-06-30 16:30:15
- **Source:** my_project

(Content of README.md)

---

# script

## Metadata
- **Generated on:** 2024-06-30 16:30:16
- **Source:** my_project

(Content of script.py)

---

# data

## Metadata
- **Generated on:** 2024-06-30 16:30:17
- **Source:** my_project

(Content of data.json)

---

# styles

## Metadata
- **Generated on:** 2024-06-30 16:30:18
- **Source:** my_project

(Content of styles.css)
```

