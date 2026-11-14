# Ebonefire — Project Instructions

Ebonefire is a pre-alpha dark-fantasy game targeting Godot 4.x.

## Work carefully
- Inspect the existing project before changing it; preserve existing work.
- Do not invent game mechanics, story details, controls, art direction, or assets.
- When requirements are unclear, make the smallest reversible change and document assumptions.
- Keep changes focused and explain what changed and what remains unverified.

## Godot 4 conventions
- Use Godot 4.x and GDScript 2.0; avoid Godot 3 APIs.
- Prefer typed GDScript, snake_case names, tabs for indentation, reusable scenes, and small scripts.
- Use signals for decoupled communication and exported properties for tunable values.
- Do not add plugins or third-party assets without approval.

## Layout
- `scenes/` — scenes.
- `scripts/` — shared scripts.
- `assets/` — art, audio, fonts, and source assets.
- `resources/` — reusable resources.
- `docs/` — project and technical notes.

## Verify
When Godot is installed, run:
- `godot --headless --path . --editor --quit`
- `godot --headless --path . --quit`

If Godot is unavailable, perform static checks and state that runtime verification was not possible. Never claim unrun tests passed.

## Git and secrets
- Never commit credentials, API keys, personal data, or local editor state.
- Do not delete user assets as cleanup.
- Do not force-push or rewrite history.
- Do not commit unless the owner explicitly requests it.

## Current state
The initial scaffold is only a launchable project foundation. The final game dimension (2D/3D), mechanics, and content are not yet established; do not assume them.
