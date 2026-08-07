# Contributing a Course Guide

Guides here are written by FAST NUCES Karachi students, for the students who come after them. No guide is "official" — it's just what worked, from someone who actually sat the exam.

## Before you start

- One guide per course, at `guides/<COURSE_CODE>/guide.md` (e.g. `guides/CS2005/guide.md`).
- If a guide already exists for your course, don't start a new one — open a PR against the existing file instead (see "Editing an existing guide" below).
- Write from your own experience. Don't invent facts, links, exam formats, or professor names you're not sure about — it's fine to leave a section as "(leave for someone else to fill in)".
- No file uploads here — this repo is for guidance and links, not resources. If you have notes, past papers, slides, etc. to share, upload those through Trek's normal resource contribute flow instead, then just point to them by category name in your guide (e.g. "check the Past Papers section").

## Writing a new guide

You have two options — pick whichever's easier for you.

**Option A — draft it with AI.** Copy the ready-made prompt from the "Draft it with AI" button on your course's Guide tab on Trek, paste it into ChatGPT, Claude, or any AI chat, and answer its questions about the course. It'll hand you back a complete guide in the right format — paste that into the file in Step 3 below.

**Option B — write it yourself.** Use the "Start on GitHub" button on Trek, which opens a prefilled blank template for your course directly on GitHub. Fill it in and skip to Step 4.

### Steps (if starting from scratch, i.e. not using the "Start on GitHub" button)

1. **Fork this repo** — click "Fork" in the top right of the repo page. This gives you your own copy to work in.
2. In your fork, create `guides/<COURSE_CODE>/guide.md` (make the folder if it doesn't exist).
3. Paste in your guide content — either your own writing, or what an AI chat gave you from the prompt in Option A above.
4. Commit the file.
5. Open a **pull request** back to this repo: go to your fork, click "Contribute" → "Open pull request", add a short description, and submit.

That's it — a maintainer will review and merge it. Once merged, it shows up on Trek automatically (may take a few minutes for the cache to clear).

## Editing an existing guide

Click "Suggest an Edit" on the course's Guide tab on Trek — it opens the file directly in GitHub's editor. Make your changes, then GitHub will walk you through forking (if you haven't already) and opening a PR, same as above.

## Style

- Sound like a student talking to the next batch, not a textbook or marketing copy. Direct, concrete, specific.
- Prefer real specifics ("the recursion-tree method is what actually saves you on the exam") over vague advice ("practice makes perfect").
- Keep it skimmable — short paragraphs, real bullets, no walls of text.
- Keep the heading structure intact (`## Overview`, `## Topics & Resources`, etc.) — Trek parses these to render the guide, so renaming or removing them will break formatting.

## Questions

Open an issue on this repo, or ask us.