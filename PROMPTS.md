# Prompts for the workshop

Copy, paste, and adapt. Notice how each prompt gives the model **purpose, sources, constraints, and the output you want**.

---

## Track A: The Claude app

Attach `data/worldphones.csv` to a new chat first.

### 1. Understand the data before analyzing it

> This CSV counts telephones (in thousands) in seven world regions for 1951 and 1956–1961. Before any analysis, describe the dataset: its columns, units, years covered, and any gaps or limitations a careful researcher should know about.

### 2. Bring in current data

> Now find current figures on the number of telephone lines in use by country. Use Wikipedia's "List of countries by number of telephone lines in use" or a comparable ITU source. Tell me exactly where the numbers came from and what year they refer to.

### 3. Analyze and visualize

> Create a chart comparing telephone access in 1961 with today, for a master's seminar on the digital divide. Show your calculations. Then give me three discussion questions, including one about what landline data cannot tell us about connectivity today.

### 4. Add the skill, then compare

Upload `skills/sis-data-brief.zip` in the Skills section of Claude's settings, start a new chat, attach the CSV, and ask:

> Prepare a data brief on this dataset for an SIS lecture.

**Reflect:** What changed when Claude had your method in writing?

### 5. Verify

> Which of the figures you gave me should I double-check, and how? List the source for each one.

---

## Track B: Positron and Posit Assistant

Open `workshop-starter.qmd` and the Posit Assistant panel.

### Getting oriented

> Explain what each code chunk in workshop-starter.qmd does, in plain language, for someone who has never used R.

### Clean the scraped table

> The `today` table from Wikipedia has numbers stored as text with commas. Write code that converts the telephone line counts to numbers, and add it as a new chunk in section 5.

### Make a new chart

> Make a horizontal bar chart of the 15 countries with the most telephone lines in the `today` table, and add it to the document with a short explanation.

### Connect then and now

> Add a paragraph comparing the 1961 regional totals with today's top countries. Be explicit about the limits of comparing regions with countries, and landlines with overall connectivity.

### When something breaks

> I got this error: [paste the error]. What does it mean, and how do I fix it?
