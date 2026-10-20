# AI English Lessons

Ready-to-teach English lessons for B1–B2 adult learners, built each week from the AI newsletter *AI Trend Search*.
Live site: https://hazajous-code.github.io/ai-english-lessons/
Source newsletter: https://hazajous-code.github.io/ai-newsletter-en/ (Korean edition: https://hazajous-code.github.io/ai-newsletter-claude/trend/)

## Structure
- `index.html` — current lesson, teacher's guide (lesson plan, answer keys, teacher's notes, sources)
- `student.html` — current lesson, student handout (no answers; printable)
- `lessons/<YYYY-MM-DD>.html`, `lessons/<YYYY-MM-DD>-student.html` — permanent copies (shared-page links use `../`; the pair link to each other)
- `archive.html` — past lessons (entries added by `promote.py`)
- `style.css` — the newsletter's stylesheet plus lesson and print styles at the end

## Each lesson (75 min, B1–B2 adults)
Teacher's guide: lesson at a glance (level, time, objectives) → 01 lesson plan table → 02 warm-up → 03 vocabulary (12 words: word, part of speech, meaning, example from the text) + gap-fill with answer key → 04 reading (adapted text, about 500 words, 3–4 titled parts) → 05 comprehension (4 true/false + 4 short answer) with key → 06 language focus (one grammar or functional point drawn from the text, explanation, examples from the text, two tasks with keys) → 07 discussion (6 questions) → 08 role-play (setup, three role cards, useful language) → 09 writing task → 10 teacher's notes (focus point, pronunciation, common error, lower/higher-level adaptations) → sources.
Student handout: the same without lesson plan, answer keys, teacher's notes and sources; with a print button and writing lines.

## Content rules
- The reading text adapts the English edition of the same week's newsletter issue. Use only facts, numbers, dates and caveats that appear in that issue; keep claims marked as claims and estimates as estimates. Simplify language, not facts.
- Grade the language for B1–B2: mostly common vocabulary, sentences under ~25 words, no unexplained jargon (explain technical terms in the text or the vocabulary list).
- Vary the language focus each week (e.g., passive voice, reporting verbs and hedging, conditionals, comparatives, modal verbs, phrasal verbs, linking words).
- Discussion and role-play should suit adult professionals and avoid personal or sensitive topics.

## Publishing
Lessons are generated from the newsletter every Tuesday (KST), after the English edition is published. `promote.py` (run daily by `.github/workflows/daily.yml`) moves lessons listed in `scheduled.json` to the front page on their date.
