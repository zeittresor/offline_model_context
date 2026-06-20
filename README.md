# Offline Model Update Bundle v5 — 2026-06-20

Purpose: model-agnostic offline/local AI context bridge. These files provide a dated external context snapshot from 2024-06-01 through 2026-06-20. They do not permanently update any model.

Public project/reference: https://github.com/zeittresor/offline_model_context
License note: The user's public project is MIT-licensed. This generated bundle is intended to follow the same general offline-model-context idea; verify license headers before redistribution if you modify it.

Recommended use:
- Small models / small context: start with `context_only.md` or `full_8k.md`.
- 16k/32k models: use `full_16k.md` or `full_32k.md`.
- 64k/128k/256k models: use the matching `full_*k.md` variant.
- RAG/indexed systems: use `cards_context_only.jsonl`, `event_index.md`, and `weekly_chronology.md`.
- Human/online audit: use `source_registry.md`; raw URLs are kept there, not in the main offline-facing context files.

No PDF. No images. Markdown/Text/JSONL only.

Important: token counts are approximate context-window classes, not exact tokenizer-specific counts. Keep room for system prompt, user query and answer output.
