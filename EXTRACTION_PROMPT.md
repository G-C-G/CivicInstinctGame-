# Portfolio extraction prompt

Run once per project, in a session that has that project's files.

You are extracting evidence for a creative portfolio case study. Your job is to report what the project files show. Do not write marketing copy and do not fill gaps.

## Rules
1. Use only what is in the files, commits, docs and assets I've given you. Every claim must name its source (file path, commit or document).
2. Label every statement as one of: **VERIFIED** (stated directly in a source), **INFERRED** (reasonable reading, say what it's based on) or **MISSING** (needed but not in the files).
3. Never invent clients, users, results, dates, awards, revenue, testimonials or capabilities. If there are no results, write "No results recorded".
4. Separate what was **planned** from what was **built**, and what was **built** from what was **used by real people**. Sample or test data is not usage.
5. Don't assume authorship. Git author names, AI tool use and collaborators must be reported as found, and the question "who actually did what?" must be listed under MISSING.

## Report, in this order
1. **Snapshot:** name, one-sentence description, category, status (idea, prototype, built, in beta, live), dates (from files), and the evidence for each.
2. **Problem and opportunity:** what it was made to solve, in the files' own words where possible.
3. **Core concept and mechanics:** how it works, in plain language. Then list every design decision or rule the files state, such as what was left out on purpose and why.
4. **Contribution map:** a table of people and tools, what each did according to the sources, and what's MISSING. Include commit authors and any named collaborators.
5. **Technology:** stack, hosting and integrations, kept to a level a non-technical reader could follow. Mark separately anything that is internal operations (costs, accounts, workarounds) and should NOT appear in a portfolio.
6. **Process:** how it evolved, using commit history or dated documents. Note the strongest decisions or turning points.
7. **Results:** only measured outcomes with a source. Otherwise write "none recorded" and list which metrics could be tracked.
8. **Challenges and solutions:** only those documented in the files.
9. **Asset inventory:** a table of every screenshot, video, diagram, document and demo, with file path, what it shows, quality (usable, needs a retake), and a flag if it shows real personal data, client names or confidential material.
10. **Publishing risks:** real names, private data, client confidentiality, unreleased IP, sample vs real data, and any claim that could embarrass me if someone checked.
11. **Gaps and questions for me:** a numbered list of everything MISSING, ordered by how much it blocks the case study.
12. **Proposed positioning:** two options for the strongest honest angle, each with the evidence behind it and the weakest assumption in it.

Output as clean markdown with tables where noted. End with a one-line status: ready for case study, needs my answers first, or not enough evidence.

## How to use it
- Run it separately on each project so reports stay comparable, then feed the reports into the portfolio build.
- Answer the "Gaps" list yourself, especially contribution and results. Those two sections decide whether the portfolio is credible.
- For projects outside a repo (decks, photos, Canva files, old phones), paste in or upload what you have and add a one-line note on where each item came from.

**Weakest assumption:** that the files tell the whole story. For most projects, the real evidence is in your memory and in people's messages, not the folders. So the Gaps list matters more than the report.
