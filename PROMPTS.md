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

Open `workshop-starter.qmd`, then open Posit Assistant (Command Palette → **View: Show Posit Assistant**). Work through these six prompts in order. **Read every change before you accept it.**

### 1. Orient

> What do you know about this project? Who is the audience, and what standards should you follow?

*It should mention the SIS workshop and the research standards in `AGENTS.md`. If it doesn't, the folder isn't trusted.*

### 2. Explain

> Explain section 3 of workshop-starter.qmd line by line, for someone who has never used R.

### 3. Fix (whenever you hit an error)

> I got this error: [paste the error]. What does it mean, and how do I fix it?

### 4. Extend

> The today table stores numbers as text with commas. Add a chunk in section 5 that converts them to numbers.

### 5. Plan

> /plan Add a bar chart of the 15 countries with the most telephone lines, with a short explanation.

*Starting with `/plan` asks the Assistant to propose a plan before it changes anything.*

### 6. Interpret

> Draft a paragraph comparing 1961 regions with today's leaders. Flag what landline data can't tell us.

Then click **Preview** and look at what you built: prose, code, and output together. Which parts would you cite? What would you check first?
