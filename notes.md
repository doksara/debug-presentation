# Notes

<!--
Entry template — copy below for each new entry:

## <Title>
- **URL:** <link>
- **Date:** YYYY-MM-DD
- **Key points:**
  - <point 1>
  - <point 2>
  - <point 3>
-->

## Vertical Slice Architecture for Web Apps

- **URL:** https://cleancodeguy.com/blog/vertical-slice-architecture
- **Date:** January 6, 2026
- **Key points:**
  - Vertical slice architecture organizes code by business feature rather than technical layer
  - That reduces context switching, lowers integration bugs, and helps teams deliver value faster.
  - AI-friendly codebases -> AI coding assistants work best with tight, relevant context. When a slice contains UI, API, and data code for a feature, AI tools can offer much more accurate suggestions because the context window is coherent and focused. In layered systems, scattered context often produces generic or incorrect suggestions from tools like GitHub Copilot.
  - Vertical slices bring clarity, but watch for these anti-patterns:
  - The “fat” slice — one slice grows to cover many features. Fix by splitting into smaller, single-purpose slices.
  - Leaky business logic — rules placed in shared. Fix by moving business rules back into the slice they belong to.
  - Inconsistent slice structure — different folder layouts across features. Fix by agreeing on project conventions for naming and structure.

## Most devs don’t understand how context windows work

- **URL:** [<link>](https://www.youtube.com/watch?v=-uW5-TaVXu4)
- **Date:** YYYY-MM-DD
- **Key points:**
  - "lost in the middle" -> in large prompts, information at the start and end is prioritized
  - context window -> input tokens + output tokens in a session
