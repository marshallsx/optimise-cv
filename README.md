# CV Optimiser — a Claude skill

Tailors a CV to a specific job description before you apply. Built by Scott Marshall as part of the "Build with AI" series; the starting point was a set of career-coach prompts shared on LinkedIn, merged into one process with guardrails added.

What it does, in order: a recruiter-eye audit (top five problems, ranked), a requirement-by-requirement evidence map with a fit score out of 10 and an Apply / Apply with caveats / Don't apply verdict, honest keyword gaps (only terms your CV supports get added), bullet rewrites, three summary options, and a tailored CV as a Word document with a change log of every edit.

Guardrail: it never invents facts or numbers. Where a metric would help but isn't on your CV, it writes `[ADD METRIC: ...]` and leaves it for you.

## How to use it

1. Download SKILL.md.
2. In Claude Cowork or Claude Code, add it as a skill (Cowork: Settings → Skills → add; Claude Code: create a folder called cv-optimiser inside ~/.claude/skills/ and put SKILL.md in it).
3. Start a chat, attach your CV and the job description, and say "optimise this CV for this job".

UK conventions by default (two pages, British spelling, no photo). Ask it to switch if the role is elsewhere.

Free to use and adapt. If you improve it, I'd like to hear about it.
