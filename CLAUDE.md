# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Python Data Science Handbook built with Quarto, serving as a comprehensive educational resource. The project is structured as a Quarto website that renders HTML documentation from QMD (Quarto Markdown) files with embedded Python code.

## Essential Commands

### Development and Preview
```bash
# Preview the website locally (most common development task)
quarto preview index.qmd --no-browser --no-watch-inputs

# Preview with browser and watch inputs (for live development)
quarto preview index.qmd

# Render the entire site
quarto render

# Render specific file
quarto render path/to/file.qmd
```

### Git Operations
```bash
# Restore deleted content (common issue with sidebar references)
git checkout HEAD -- "directory_name/"

# Check git status for QMD files
git status | grep "\.qmd"
```

## Architecture and Structure

### Quarto Configuration
- **Main config**: `_quarto.yml` defines website structure, sidebars, and themes
- **Custom filters**: `foldableCodeBlock.lua` provides collapsible code blocks
- **Output directory**: `docs/` contains the rendered HTML site
- **Freeze cache**: `_freeze/` stores computational results for faster builds

### Content Organization
The site is organized into logical sections, each with its own directory:

- **`intro/`**: Basic Python concepts and setup
- **`data manipulation/`**: Pandas, SQL, data structures, I/O operations
- **`plot/`**: Visualization libraries (Seaborn, Plotnine, Plotly)
- **`Publish/`**: Shiny and Quarto publishing workflows
- **`other/`**: Advanced topics like web scraping

### Sidebar Structure
The website uses 5 main sidebars defined in `_quarto.yml`:
- **intro**: Introduction and basic concepts
- **bar0** (Data): Data manipulation content
- **bar1** (Plotting): Visualization libraries
- **bar2** (Publish): Publishing and sharing
- **bar7** (Other): Advanced topics and web scraping

### Code Execution Pattern
- All Python code blocks use ````{python}` syntax (not ````python`)
- Code execution is configured with `execute: freeze: auto` for caching
- Common code execution settings in frontmatter:
  ```yaml
  execute:
    warning: false
    error: false
    cache: true
  ```

## Development Guidelines

### File Management
- **QMD files**: All content should be in QMD format for Quarto processing
- **Python code**: Always use ````{python}` blocks with proper syntax
- **File references**: When directories are referenced in `_quarto.yml`, they must exist and contain QMD files
- **Deleted content**: If sidebar references break, restore content with `git checkout HEAD`

### Code Examples
- **Real URLs**: Use actual working websites (e.g., `books.toscrape.com`) not placeholder URLs
- **Error handling**: Include proper exception handling in web scraping examples
- **Complete functions**: Provide full function implementations, not just function calls
- **Commented examples**: Use commented code for examples that shouldn't execute during rendering

### Common Issues and Solutions
1. **Sidebar errors**: If sidebars fail, check that referenced directories contain QMD files
2. **Missing content**: Use `git checkout HEAD -- "directory/"` to restore accidentally deleted content
3. **Lua filter errors**: Ensure `foldableCodeBlock.lua` exists and matches the reference in `_quarto.yml`
4. **Python execution errors**: Verify all Python code blocks use `{python}` syntax and have proper imports

## Dependencies and Environment

The project assumes these Python packages are available:
- requests, beautifulsoup4, selenium (web scraping)
- pandas, numpy (data manipulation)
- matplotlib, seaborn, plotly, plotnine (visualization)
- quarto (document rendering)

## Deployment

- **GitHub Pages**: Site deploys to `https://jcfly3000.github.io/Into-Python/`
- **Output**: Built files go to `docs/` directory
- **Theme**: Uses Cosmo theme with custom styling from `styles.css`