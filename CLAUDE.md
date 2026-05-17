# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repo is

A **presentation asset repo**, not a software project. It holds source/export files for a talk on frontend architecture and Feature-Sliced Design (FSD), plus the research notes and diagrams that back it.

There is no build, no test suite, no package manager, no application code. Do not look for one.

## Layout

- `frontend-arhitektura--dark-tech-with-fsd.key` / `.pptx` / `.pdf` — the main deck (Keynote source + PowerPoint and PDF exports). The Keynote file is the source of truth; the `.pptx` and `.pdf` are exports that may lag behind.
- `fsd-layers-modern-dark.key` — a secondary/auxiliary deck on FSD layers (Keynote only).
- `static/` — PNG diagrams embedded in the deck (FSD layer diagrams, folder graphics). When the deck references a diagram, the source PNG lives here.
- `notes.md` — research notes feeding the talk. Uses a fixed entry template (Title / URL / Date / Key points) — preserve it when adding new entries.
- `LLMs.txt` — full Feature-Sliced Design documentation, kept locally as an offline reference for the talk's content. Treat it as read-only source material, not as something to edit.

## Working in this repo

- Binary deck files (`.key`, `.pptx`, `.pdf`) cannot be meaningfully edited via tools here — open them in Keynote/PowerPoint. If a user asks for "slide changes," the expected output is usually edits to `notes.md`, `static/` assets, or guidance the user will apply manually in Keynote.
- When the topic is FSD methodology questions, prefer the `feature-sliced-design` skill and/or `LLMs.txt` over web search — the local copy is the canonical reference the talk is built against.
- `.DS_Store` is the only ignored file; the deck exports (`.pdf`, `.pptx`) **are** tracked intentionally so reviewers without Keynote can read the talk.
