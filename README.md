# Beyond the Chatbot: From Claude to Code with Positron

**SIS Faculty AI Training Series, Session 2**
School of International Service, American University
Facilitator: Dr. Derrick L. Cogburn

Welcome! This repository (or "repo") holds everything you need for today's hands-on workshop. You don't need any coding experience. If a term below is new to you, see the glossary at the end of this page.

---

## The idea in one sentence

We'll take one research question and work it two ways, first in the **Claude app** and then in **Positron** (a free tool for working with code), so you can see what each approach offers and decide which one fits your work.

## Our shared question

> What does the global distribution of telephone access, then and now, tell us about the digital divide, and what can't these data tell us?

- **Then (1951–1961):** `WorldPhones`, a small historical dataset that ships free inside R. It counts telephones (in thousands) in seven world regions for 1951 and 1956–1961.
- **Now:** current figures scraped live from Wikipedia's *List of countries by number of telephone lines in use*, which draws heavily on ITU (International Telecommunication Union) data.

---

## What's in this repo

| File or folder | What it is | Which track |
|---|---|---|
| `README.md` | This page: instructions and glossary | Everyone |
| `PROMPTS.md` | Ready-to-use prompts for both tracks | Everyone |
| `data/worldphones.csv` | The WorldPhones data as a spreadsheet file you can upload to Claude | Claude app |
| `skills/sis-data-brief/SKILL.md` | A sample **skill file**: written instructions that teach Claude a method | Claude app |
| `skills/sis-data-brief.zip` | The same skill, zipped and ready to upload to Claude | Claude app |
| `workshop-starter.qmd` | The Quarto document we'll run and extend in Positron | Positron |
| `AGENTS.md` | An **agent file**: standing project instructions Posit Assistant reads automatically | Positron |

---

## Getting the files

### Option 1: Clone with Git in Positron (recommended)

"Cloning" simply means downloading a copy of the repo that stays linked to the original.

1. Open **Positron**.
2. Choose **File → New Folder from Git...**
3. Paste this repo's web address (the URL in your browser's address bar) and press Enter.
4. Choose where to save it (for example, your Documents folder).
5. When asked, open the folder and choose **Yes, I trust the authors**. (Posit Assistant only reads `AGENTS.md` in trusted folders.)

### Option 2: No Git? Download a ZIP

1. On this page, click the green **Code** button, then **Download ZIP**.
2. Unzip the file.
3. In Positron, choose **File → Open Folder...** and select the unzipped folder.

Either way, you end up with the same files.

---

## Track A: The Claude app

You only need a web browser and a Claude account.

1. Download `data/worldphones.csv` (click the file, then the download icon).
2. In Claude, start a new chat, attach the CSV, and try the prompts in `PROMPTS.md`.
3. **Add the skill:** download `skills/sis-data-brief.zip`, then upload it in the **Skills** section of Claude's settings. Run the same prompt again and compare the results.

## Track B: Positron

### One-time setup (5 minutes)

In Positron's **Console** (the pane where R runs), paste this line and press Enter:

```r
install.packages(c("tidyr", "ggplot2", "rvest", "rmarkdown", "knitr"))
```

### Connect Posit Assistant to Claude

1. Open the Command Palette: **Cmd+Shift+P** (Mac) or **Ctrl+Shift+P** (Windows).
2. Run **Posit Assistant: Configure AI Providers**, then choose **Connect** next to **Anthropic** and paste your API key.
3. Run **View: Show Posit Assistant** to open the chat panel.

Treat your API key like a password: never put it in a file in this repo, an email, or a shared document.

### Run the document

1. Open `workshop-starter.qmd`.
2. Run one chunk at a time with the **Run Cell** link above each grey code block, or render the whole document with **Preview** (**Cmd/Ctrl+Shift+K**).
3. Work through the "Your turn" sections with Posit Assistant.

---

## A note on Python

Today's starter file uses **R** because it installs more predictably on a room full of different laptops. Positron works just as well with **Python**, and the facilitator's demo shows the same workflow in Python (with pandas and Beautiful Soup). Python can be covered in a future session or by request.

---

## Plain-language glossary

| Term | Meaning |
|---|---|
| **LLM** (Large Language Model) | The kind of AI behind Claude: trained on large amounts of text to understand and generate language. |
| **GUI** (Graphical User Interface) | A point-and-click app, like the Claude website or desktop app. |
| **Context** | Everything the model can "see" at once: your prompt, files, and instructions. |
| **Skill file** (`SKILL.md`) | A plain-text file of reusable instructions that teaches Claude how to do a task your way. |
| **Agent file** (`AGENTS.md`) | A plain-text file of standing project instructions an AI assistant reads automatically. |
| **API** (Application Programming Interface) | A structured way for one program (Positron) to ask another (Claude) for help. |
| **API key** | A secret code that identifies you when a program uses an API, so usage can be tracked and billed. |
| **IDE** (Integrated Development Environment) | A workspace for writing and running code. Positron is an IDE. |
| **R** | A free programming language for statistics and data analysis. |
| **Quarto** (`.qmd`) | A document format that combines prose, code, and results; renders to Word, PDF, web pages, or slides. |
| **Chunk** | A grey block of code inside a Quarto document. |
| **CSV** (Comma-Separated Values) | A simple spreadsheet file almost any program can open. |
| **Git / GitHub / repo** | Git tracks versions of files; GitHub hosts them online; a repo is one project's folder. |
| **Web scraping** | Using a program to collect information from web pages automatically. |

---

*Data: `WorldPhones` from the R `datasets` package (source: AT&T, The World's Telephones, 1961). Current figures from Wikipedia. Always verify before citing.*
