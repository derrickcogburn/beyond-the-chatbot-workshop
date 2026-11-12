# Project instructions for Posit Assistant

Posit Assistant reads this file automatically when this folder is open in Positron (and trusted). It works like an "agent file": standing instructions for the whole project.

## About this project

- This is a hands-on workshop for faculty and doctoral students at American University's School of International Service (SIS).
- Most participants are **new to R and to coding**. Some are skeptical of AI tools.
- The research question: what does the global distribution of telephone access, then (1951–1961) and now, tell us about the digital divide?
- Data: `WorldPhones` (built into R; telephones in thousands by region) and a table scraped from Wikipedia's "List of countries by number of telephone lines in use."

## How to help

- Explain code in **plain language** and define any technical term the first time you use it.
- Prefer **simple, readable tidyverse-style R** (tidyr, ggplot2, rvest) over clever or compact code.
- Add code to `workshop-starter.qmd` as new Quarto chunks, each with a `#| label:` line as the first line inside the chunk.
- Explain each change you make to the document before or after the code.

## Research standards

- State the source, units, and year of every figure.
- Flag missing data and limitations; never infer causation from descriptive trends.
- Be explicit when comparing regions (1961) with countries (today), and landlines with overall connectivity.
- If you are unsure about a number or a source, say so rather than guessing.
