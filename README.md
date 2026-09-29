# Open Textbook Draft

An AI skill that guides an author from a rough idea to a complete open textbook draft, entirely through conversation. You talk; the skill proposes, drafts, checks, and keeps the project files up to date.

Created by David Wiley.

## What it does

The skill walks you through nine phases. You approve each one before the next begins.

1. **Purpose, audience, and landscape:** why the book should exist, who it's for, and what's wrong with existing books
2. **Style guide:** reading level, voice, kinds of examples, formative and summative practice, accessibility and sourcing rules
3. **Chapter list:** how many chapters, and what they're called
4. **Table of contents in three passes:** headings at each level, with a learning outcome for every top-level section and a check that every outcome is taught and assessed
5. **Chapter drafting:** Chapter 1 first, a stress-test chapter, then a frozen chapter template that every later chapter follows
6. **Knowledge-graph audit:** a map of every concept in the book, checked for concepts used before they're introduced, circular prerequisites, and gaps in coverage
7. **Figures, photos, video, and interactives:** suggestions and builds, with every external resource logged for attribution
8. **Front and back matter:** preface, glossary, license page, AI-use statement, instructor materials, and a pilot plan
9. **Title and subtitle:** workshopped last, once the content is known

## What you need

An AI tool that supports skills (folders containing a `SKILL.md` file) and can read and write files in a project folder. Tools that support skills include:

- **Claude Code**
- **OpenAI Codex**

Other tools have adopted the same format, so check yours. Working in a folder on your computer is best: the skill keeps its progress files there, which is how it picks a book back up in a later session.

Web search is helpful for the landscape scan and for verifying links, but it's optional. The skill says so plainly whenever it couldn't check something.

## Installing

**OpenAI Codex: just ask.** In a chat, say:

> Install the skill at github.com/kalendar/open-textbook-draft

Codex's built-in skill installer downloads it from GitHub, and it's available on your next turn.

**Claude Code:** the skill needs to live in a skills folder: `~/.claude/skills/` for all your projects, or `.claude/skills/` inside one project. You can ask Claude Code to clone this repo into that folder for you.

**Claude on the web:** download this repo as a zip and upload it in Settings (look for the skills section; the menu name changes from time to time). This requires a paid plan with code execution enabled. Make sure the folder inside the zip is named `open-textbook-draft`. GitHub's "Download ZIP" names it `open-textbook-draft-main`, so rename it before zipping if needed.

Skills you add in one Claude product don't carry over to the others, so repeat the step for each one you use.

## Starting a book

Start a new conversation and say something like:

> I want to write an open textbook for my introductory statistics course. Can you help me get started?

To come back to a project later, open a conversation in the same project folder and say:

> Help me pick up my textbook where we left off.

The skill keeps its own record of progress and decisions, so it can pick up where you stopped.

## Files it creates

The skill creates and maintains these in your project folder: a progress log, a decision log, a book brief, a style guide, an outline, a chapter template, one file per chapter, a glossary, an example bank, an attribution ledger, and the knowledge graph (`knowledge-graph.json`) with a plain-language audit report.

## Principles

- **You decide.** The skill proposes and never advances a phase without your approval.
- **No invented sources.** Claims that need support are marked for you to check, and unverified links are labeled.
- **Honest about limits.** If it estimated something instead of computing it, or didn't run a search, it says so.

## Licensing

**This skill** is licensed under [Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/). You may share and adapt it, including commercially, as long as you credit David Wiley, indicate any changes, and license your adapted version under the same terms. Contributing your improvements back to this repo makes the skill better for everyone! If you need technical support for contributing your changes, ask your AI to help you or email David.

**Books made with this skill are not "adaptations" of the skill for purposes of the license**, and you choose how to license your books. During the process the skill will discuss options with you and recommend CC0 1.0 as a default, because purely AI-generated text generally isn't eligible for copyright protection in the U.S. (while your own writing, edits, and choices in selecting and arranging material may be). This is not legal advice. Rules differ by country.
