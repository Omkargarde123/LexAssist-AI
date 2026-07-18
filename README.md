# LexAssist AI — Live Demo

A fully client-side, offline-capable Indian legal information assistant. No API key, no backend, no network calls — everything runs in the browser against an embedded knowledge base.

## What's inside

The knowledge base is parsed from a 15-chapter "AI Legal Knowledge Base" reference document covering:

- The Constitution of India
- Bharatiya Nyaya Sanhita (BNS), Bharatiya Nagarik Suraksha Sanhita (BNSS), Bharatiya Sakshya Adhiniyam (BSA)
- Consumer Protection Act, Companies Act, IT Act, GST, Income Tax, Labour Codes
- 37 landmark Supreme Court / High Court judgments
- 122 FAQ entries
- Government notifications & compliance guidance

In total, **293 indexed passages** are embedded directly in the page and searched with on-device keyword matching (no LLM, no API).

## Features

- **AI Legal Chat** — ask a question, get an answer assembled from the closest matching knowledge base passages, with citations.
- **Contract Review** — paste contract text; a heuristic scanner flags missing standard clauses (termination, indemnity, liability, IP, dispute resolution, etc.) and risky one-sided language.
- **Compliance Checker** — checklist-based gap check against GST, Companies Act, Labour Codes, or IT Act requirements.
- **Case Research** — search the embedded landmark judgments (Facts / Issue / Decision / Significance).

## Running it

Just open `index.html` in any browser — no build step, no server, no dependencies.

To serve it locally:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Disclaimer

This tool provides general legal information for educational purposes only. It is not a substitute for advice from a licensed lawyer. Always verify current provisions against official government sources.
