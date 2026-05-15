# Working with Documentation and mkdocs.yml

## Getting started

To begin working with your repository's documentation, navigate to the `/docs` folder.

This folder already contains initial content from the repository onboarding, which you can either replace entirely or expand upon by adding new Markdown (`.md`) files.

## Editing Documentation

- Add or edit Markdown (`.md`) files in the `docs/` directory.  
- The main entry point is `docs/index.md`.  
- Use headings to organize content; only one H1 (`#`) per file.

The Table of Contents on the right is generated automatically based on the hierarchy  
of headings. Only use one H1 (\`\#\` in Markdown) per file.

## Configuring mkdocs.yml

- The `mkdocs.yml` file in the repository root configures the documentation site generated on the Engineer Workbench portal.  
- You can set the site name, description, and navigation.  
- To customize navigation, add a `nav` section in `mkdocs.yml`:

```
nav:
  - Home: index.md
  - Another Page: another-page.md
```

- For more options, see the [MkDocs configuration guide](https://www.mkdocs.org/user-guide/configuration/).

## Publishing Docs

- The techdocs annotation in `catalog-info.yaml` is already uncommented:

```
annotations:
    backstage.io/techdocs-ref: dir:.
```

- After your changes are merged into the main branch, documentation updates will be automatically synced and published to the Engineer Workbench portal.

## Quick Start

**How to Update Documentation**

To make changes or additions to the documentation:

The process for updating component technical documentation involves the following steps:

1. **Create a New Branch.**  
2. **Edit Documentation Files:** Modify or add Markdown files within the `docs/` directory.  
3. **Update Configuration:** Adjust `mkdocs.yml` as needed.  
4. **Preview (Optional):** Locally verify your changes using `mkdocs serve` (requires MkDocs installation).  
5. **Submit for Review:** Push your branch and open a Pull Request (PR).  
6. **Complete the PR.**  
7. **Automatic Update:** Once the PR is completed, your component documentation updates will be automatically published to the Engineer Workbench portal.
