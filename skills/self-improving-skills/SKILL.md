---
name: self-improving-skills
description: Use after finishing any deliverable made with a skill (a video, a page, a document, a script) or when starting a kind of task no skill covers yet. Asks the user for feedback, writes the lessons back into the right skill or memory, and looks online for existing skills that would fill a gap, asking the user before installing anything. Turns every finished task into a better skill for the next one.
---

# Self-improving skills

Every session starts from zero. The only learning that lasts is what gets written into skill files and memory. This skill is the loop that does the writing, so the user does not have to track it.

## When to run

- A deliverable made with a skill is done and the user has seen it.
- The user corrects you, praises something, or says "do it like last time".
- A new kind of task comes up and no installed skill covers it.

## The loop

### 1. Ask for feedback (never skip)
Ask one short question: "What did you like, what should change?" Wait for the answer. Do not guess the feedback yourself.

### 2. Sort each lesson into the right place
- **How to do the task** (a step, a setting, a bug and its fix, a style that worked) → the skill that was used, in a short "Lessons" section.
- **Who the user is** (taste, goals, budget, tools they dislike) → memory, not the skill.
- **Neither** → drop it.

Before writing, ask yourself: "Will this help the next time this skill runs?" If no, do not write it.

### 3. Write it small
- One line per lesson, concrete. Good: "Subtitles too small, use 90px." Bad: "User had thoughts about text."
- Merge duplicates. Keep the file short and readable.
- Write only about this skill's own job. No unrelated notes, no personal details, no lessons from a different kind of task.
- If you wrote reusable code (a component, a script), list its file path under "Reusable parts".
- Ask before deleting or reversing a major rule.

### 4. Tell the user in one sentence
"I added X to the Y skill." No long report.

### 5. Look for gaps
Ask yourself: "What is this skill missing? Is there a ready-made skill or plugin that does it?"

If yes, search. Use whatever the environment has:
- the `find-skills` skill, or `npx skills find <keywords>` ([skills.sh](https://skills.sh))
- a skill or plugin search tool, if the agent has one
- a web search for "<task> agent skill"

### 6. Offer, never install on your own
For each good match, tell the user:
- what it does for this task, in one line
- the risk (who made it, does it run code, does it send data out)
- the cost (free, paid, uses credits)

Install only after a clear yes. Then decide together whether to keep it.

### 7. No skill for a new kind of task?
Tell the user and offer to start a new skill for it. Build it from the first finished task, then let this loop grow it.

## Rules
- Feedback first, writing second. Never invent lessons.
- One skill per kind of task. Do not stuff everything into one file.
- Small and true beats long and vague.
- Tools that cost money or credits: use them only when really needed, and say why in one sentence.
