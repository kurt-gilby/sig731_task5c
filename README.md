# SIG731 Task 5C — Data Wrangling Report (Quarto QMD → PDF)

This repository contains the **Task 5C** Quarto report (`5c_task.qmd`) and the expected `data/` folder structure required to reproduce the analysis and generate the final **PDF** output.

## Repository contents


### Data location expected by the report

The report reads the dataset from:


> **Note:** The raw Stack Exchange XML files are large and are typically not committed to GitHub.  
> The recommended workflow is to download and extract the dataset locally into `./data/site/`.

---

## Recommended “one-click” build (for end users)

The intended reproducible workflow is to run an **external bootstrap Jupyter notebook** that I (the author) will provide separately (not stored in this repo). The notebook:

1. Downloads this GitHub repository as a ZIP  
2. Installs required Python packages  
3. Downloads and extracts `ai.stackexchange.com.7z` into `./data/site/`  
4. Ensures **Quarto + TinyTeX** are available  
5. Renders the report to a final **PDF**

### What the end user edits

In the bootstrap notebook, the end user sets:

```python
GITHUB_OWNER  = "<YOUR_GITHUB_USERNAME_OR_ORG>"
GITHUB_REPO   = "<YOUR_PUBLIC_REPO_NAME>"
GITHUB_BRANCH = "main"
