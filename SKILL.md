---
name: cv-optimiser
description: "Optimise a CV against a specific job description before applying: recruiter-eye audit, requirement-by-requirement fit score with an apply/don't verdict, honest keyword gaps, rewritten bullets and summary, and a tailored CV as a Word document with a change log. Use when the user shares a CV and a job spec and asks to tailor, optimise, tune, strengthen or check the CV for a role, or asks whether their CV will get past a recruiter or ATS. Not for interview preparation — that is the interview-brief skill."
---

# CV Optimiser

Takes a CV and a job description and produces (1) an honest assessment of fit and (2) a tailored CV as a Word document, with every change logged. Sits **before** the application is sent. Interview preparation is a separate skill (interview-brief) — do not drift into it.

## Inputs — both are mandatory

1. **The job description** — pasted text, a file, screenshots, or a link. If only a link is given, fetch it; if it cannot be fetched, ask for the text.
2. **The current CV** — .docx, PDF or pasted text. Read the whole file; do not work from a summary.

If either is missing, stop and ask for it. Do not guess a job description from a job title alone, and do not build a CV from memory or profile notes — the CV on file is the only source of facts about the candidate.

Optional: the user may say which sections they will not change (e.g. "leave the education section alone"). Respect that.

## Non-negotiable rules

- **Never invent facts.** No new employers, dates, titles, tools, qualifications or numbers. Where a metric would strengthen a bullet but the CV does not contain one, write `[ADD METRIC: what would help here]` and leave it for the user to fill. Every claim in the tailored CV must be traceable to the original CV or to something the user says in this conversation.
- **Keywords must be true.** Only add a term from the job description if the CV evidence supports it. If it doesn't, list it as a gap, not as an edit.
- **UK conventions by default.** "CV" not "résumé"; British spelling; no photo, date of birth or marital status; aim for two pages (three is acceptable for director-level with long careers — say when you are going over); reverse chronological; contact details at the top. If the job is outside the UK, ask before switching conventions.
- **Plain language.** Define any recruiting or HR term the first time it appears (e.g. ATS — applicant tracking system, the software recruiters use to store and search applications).
- **Honesty over encouragement.** If the CV is a weak match, say so clearly and early. The verdict comes before the rewrite.

## Process

Work through the stages in order. Stages 1–5 are the analysis and go into the report; stage 6 produces the CV.

### Stage 1 — Recruiter-eye audit (the "7-second read")

Read the CV as a senior recruiter in the job's industry who screens 200+ CVs a day for this kind of role. State exactly why they would move on in the first seven seconds. List the **top five problems, ranked by how much they hurt the candidate's chances**, and for each say what the fix is. Cover: headline/title mismatch with the role, buried or missing evidence for the job's must-haves, length and density, weak or duty-based language, dates and gaps, formatting that hides the good material.

### Stage 2 — Requirement-to-evidence map and verdict

Extract every requirement from the job description — essential and desirable, explicit and implied. For each, produce a table row:

| Requirement | Essential / Desirable | Evidence in CV (quote or section) | Strength: Strong / Partial / None | Action |

"Action" is one of: *already strong*, *surface it (move/rewrite)*, *add from CV elsewhere*, *genuine gap — do not claim*.

Then give a **fit score out of 10** with one sentence of reasoning per point lost, and a **verdict**: **Apply**, **Apply with caveats** (name them), or **Don't apply as-is** (say what would need to be true). The verdict must be defensible from the table — no softening.

### Stage 3 — Keyword and language gaps

List the exact terms, skills and tool names the job description uses that do not appear in the CV. Split into two lists:

- **True but missing** — the CV evidence supports it; show exactly where to add each term and the sentence to add it in.
- **Not supported** — do not add; these are gaps for the user to decide about.

Do not oversell the ATS: most UK recruiters still sift by hand. Keyword alignment helps a human skim, and helps searchable databases find the CV; it is not a magic gate.

### Stage 4 — Bullet rewrites

For every bullet in the roles most relevant to the job (typically the last three roles, or whatever the user specifies), rewrite using: **strong action verb + what was done + measurable result**. Keep the original bullet alongside the rewrite so the user can compare. Cut duty statements ("responsible for…") in favour of outcomes. Insert `[ADD METRIC: …]` where a number is missing and say what would strengthen it. Group rewrites by role.

### Stage 5 — Professional summary

Write three versions of the opening summary for this specific role, each under three sentences: one **confident**, one **results-focused**, one **story-driven**. Draw only on the CV. Recommend one and say why. Suggest the CV headline/title line to sit under the name.

### Stage 6 — Tailored CV (Word document)

Build the tailored CV as a .docx using the docx skill. Use the recommended summary, the rewritten bullets, the surfaced evidence and the true-but-missing keywords. Keep the user's original structure and section order unless the audit gave a reason to change it. Leave `[ADD METRIC: …]` markers in place, highlighted, so nothing is silently left blank.

Produce a **change log** as a table in the report: *Section | Original | New | Reason*. Every edit appears here — this is how the user checks that nothing was invented.

### Stage 7 — Verification before saying done

Before delivering, check and state the results:

- Every fact in the tailored CV traces to the original CV or the user's words. List any that don't and remove them.
- Every essential requirement from Stage 2 that was marked *surface it* or *add from CV elsewhere* now appears in the tailored CV.
- No term from the *not supported* list has crept in.
- Page count and UK conventions hold.
- Spelling is British throughout.

Then state plainly what was **not** checked (e.g. the job description's currency, the company's actual ATS, whether the recruiter values the same things).

## Outputs

1. **CV_Optimiser_Report_<Company>_<Role>.docx** — Stages 1–5, the change log and the verification notes. Headings in this order: Verdict and fit score; Recruiter audit; Requirement map; Keyword gaps; Bullet rewrites; Summary options; Change log; What was not checked.
2. **CV_<Name>_<Company>_<Role>.docx** — the tailored CV.
3. **In chat**: the verdict, the fit score, the top three problems, and the `[ADD METRIC]` items the user needs to fill in. No more than that — the detail is in the report.

Both files go to the user's connected folder when one is available, otherwise into the conversation.

## If the user only wants part of this

If they ask for just the audit, just the fit verdict, or just bullet rewrites, do that stage alone and offer the rest in one line. Do not produce the tailored CV unless the verdict is at least *Apply with caveats*, or the user explicitly asks for it anyway.