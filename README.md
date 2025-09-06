# Prompts Registry

## Rules
- One folder per `prompt_key`. One file per version: `vNNN.md`.
- Front-matter fields: prompt_key, env (opt), status, version, creator, tags (opt), ab_variant (opt), description (opt).
- Body contains the actual prompt text.

## Status meanings
- draft: visible to editors only; not synced as live.
- published: eligible for runtime use (DB view will expose this).
- archived: retained for history; not live.

## Environments
- dev: experimental
- staging: pre-production testing
- prod: live traffic

## Versioning
- Never edit old files for retroactive changes. Create `v00(N+1).md` and change `status`.
