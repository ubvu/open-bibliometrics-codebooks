# Open Bibliometrics Codebooks: OpenAlex & OpenAIRE

Two ready-to-run Jupyter notebooks that show, step by step, how to pull data out of two major **open, free bibliometric databases**, [OpenAlex](https://openalex.org)
and [OpenAIRE](https://www.openaire.eu), and turn it into tables and charts you can actually use.

## Why this exists

This project is a small, growing portfolio of tutorial notebooks that show **working, copy-pasteable code** for common research-evaluation tasks (look up a publication, pull everything from an institution, check data quality, and so on).

## What's inside each notebook

### `openalex_codebook.ipynb`

1. Retrieve a single work by identifier
2. Retrieve multiple works from a list of DOIs
3. All works from an institution for a given year
4. Data quality checks (retracted works, paratext, missing abstracts)
5. Using the OpenAlex Query Language (OQL) — a newer, more expressive way
   to query, including server-side grouping

API docs: [help.openalex.org](https://help.openalex.org) 

### `openaire_codebook.ipynb`

1. Retrieve a single work by identifier
2. Retrieve multiple works from a list of DOIs
3. Explore relationships for a set of DOIs (citations, dataset/software links)
4. All works from an institution for a given year
5. Data quality checks (missing DOIs, missing open-access status)
6. Boolean queries: combining `AND` / `OR` / `NOT` directly in a query

API docs: [graph.openaire.eu/docs](https://graph.openaire.eu/docs/)

## Getting started

1. **Install Python** (3.9 or later) if you don't already have it, and a way to run notebooks, [Jupyter](https://jupyter.org/install) or an editor like VS Code both work.
2. **Install the few libraries these notebooks use:**
   ```bash
   pip install -r requirements.txt
   ```
3. **OpenAlex only — get a free API key**: sign up at [openalex.org](https://openalex.org) and paste your key into the `API_KEY` variable near the top of the notebook. OpenAIRE needs no key at all.
4. **Open a notebook and run the cells from top to bottom.** Each numbered section is self-contained. Read the short explanation above each code cell, adjust the Settings if you want different data (a different DOI, institution, or year), and run it.