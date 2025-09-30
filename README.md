Miles, [30/09/2025 23:14]
Music Industry Chess

An educational, black-and-white chess experience that maps the music industry onto the chessboard.
The board = consumers (the landscape we all move across).
The pieces = roles within the industry.

This project is part of PMTWGR’s campaign around Jordy’s upcoming releases and our mantra for the season: speaks less but says more.

⸻

Why this exists
 • Inform, educate, entertain: use play to teach how the industry moves.
 • Context literacy: help artists and teams recognise power, access and incentives.
 • Public-good research: test whether games can deliver measurable learning.

⸻

Piece mapping (industry ↔ chess)

Chess Role in the industry Visual cue (b/w)
King Government / Policy Judge’s robe + crown + gavel
Queen Media / Influence Crowned sower broadcasting seeds
Rook Gatekeepers / Access points Fortified gate with arch + bars
Bishop Cultural Institution (awards, canon) Prestige trophy form
Knight Lawyers / Counsel Barrister wig + robe
Pawn Artists Hooded figure, no mouth, holding a mic like a cross

All artwork is charcoal/ink-style, monochrome, minimalist and readable on a grey board for maximum clarity.

⸻

What’s inside
 • index.html – the whole game (UI, board, moves, basic AI).
 • image/ – the black-set PNGs (transparent background). The white set is auto-derived via CSS filters unless you add separate files.
 • (Optional) assets/ – onboarding slides (PNG/JPG) if you’re using bespoke canvases for the intro.

⸻

Run it

GitHub Pages
 1. Push to main.
 2. Repo → Settings → Pages → Source: “Deploy from a branch”, Branch: main / root.
 3. Open https://<your-username>.github.io/<repo-name>/

Local (no build tools needed)
 • Double-click index.html, or serve with any static server (e.g., VS Code Live Server).

⸻

Using your art

Put your piece images here:

image/
  black-pawn.png
  black-rook.png
  black-knight.png
  black-bishop.png
  black-queen.png
  black-king.png

Important
 • Transparent PNGs, no white boxes.
 • Names must match exactly (lowercase, hyphenated).
 • If you also upload a white set, set WHITE_FROM_BLACK = false in index.html and provide white-*.png files.

Cache-busting tip
When you swap art, increment the version string in index.html (e.g., const V='?v=8' → '?v=9') so browsers fetch the new files.

⸻

AI opponents (toggle in the UI)
 • Major Label – prioritises centre control + quick returns.
 • Tech Platform – seeks disruptive trades + activity.

(ORCA/independent profile is currently disabled in code to keep the focus on the two larger “opponents.”)

⸻

Onboarding (planned, skippable)

A minimal, black-and-white intro shown before the first game:
 1. What this is – A metaphorical, playable map of the music industry’s moving parts.
 2. Sources – Mentions of public reports/research we consulted (ORCA, sector studies, PMTWGR notes).
 3. How to play – 3–5 slide micro-primer (move, capture, check, win).
 4. What we collect – light telemetry (see Privacy) + optional feedback questionnaire.
 • Consent gate for telemetry awareness.
 • Skip available (consent remains required for telemetry).

You can design the slides in Canva and export PNGs; we’ll display them full-bleed in a simple carousel.

⸻

Privacy (light-touch, GDPR-aware)

By default, the open-source build collects no personal data.
If you add analytics, keep it minimal and documented:
 • What: page views, game start/finish, number of moves, time-to-first-move, completed onboarding, optional survey answers.
 • Why: evaluate learning, improve clarity, test whether “speaks less but says more” is effective.
 • Lawful basis: Consent for analytics/surveys.
 • Storage: aggregated, pseudonymised; retention stated in the onboarding privacy note.
 • Opt-out: always available; core game still works.

⸻

Feedback & learning (optional questionnaire)

A short post-game survey (3–6 Qs) to measure clarity/impact:
 • “I can explain what each piece represents.” (1–5)
 • “This game helped me see how power moves in music.” (1–5)
 • “What confused you?” (free text)
 • “What clicked?” (free text)

Miles, [30/09/2025 23:14]
Hook this up to a simple Google Form or Airtable form; export CSV for analysis.

⸻

Roadmap
 • Onboarding carousel (with skip + consent).
 • Faster, more tactile selection highlights.
 • End-of-game summary + easy share link.
 • Optional downloadable lesson plan (teachers/mentors).
 • Accessibility pass (keyboard, ARIA, contrast).

⸻

Contributing

Issues and PRs welcome. Please keep to the monochrome aesthetic and ensure assets are transparent PNGs. For code changes, aim for small PRs with a clear before/after.

⸻

License
 • Code: MIT
 • Art: © PMTWGR. All rights reserved (no reuse without permission).

⸻

Credits

Concept & direction: PMTWGR
Art & aesthetic: PMTWGR (charcoal/ink, monochrome)
Engineering: Community + collaborators

⸻

Quick start checklist
 • index.html present at repo root
 • image/black-*.png uploaded (transparent)
 • GitHub Pages enabled (main / root)
 • (Optional) Update version cache string in index.html after swapping images
