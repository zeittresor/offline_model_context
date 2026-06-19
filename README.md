# Offline Model Update v4 - README

Created: 2026-06-19  
Coverage: 2024-06-01 to 2026-06-19  
Purpose: cumulative, dated, model-agnostic context package for local/offline LLMs.

## Recommended file choice

- Small model / small context: `full_8k.md` or `full_16k.md`.
- Medium context: `full_32k.md` or `full_64k.md`.
- Large context / RAG / analysis: `full_128k.md` or `full_256k.md`.
- Fast direct briefing: `context_only.md`.
- Concrete timeline questions: `weekly_chronology.md` plus `event_index.md`.
- RAG ingestion: `cards_context_only.jsonl`.
- Human/online audit only: `source_registry.md`.

## Important usage rule for offline models

These files are dated context snapshots, not permanent model updates. They only help when present in the prompt/context/RAG/memory system. Later real developments must be added by later-dated updates.

## URL policy

Offline-facing files contain context, not raw web links. Raw URLs are isolated in `source_registry.md` because offline models cannot open them.

## File format policy

Markdown/Text/JSONL only. No PDF. No images. No generated visuals.
