# Ebonefire

**A dark-fantasy game — pre-alpha.**

Ebonefire is being developed with **Godot 4.x**. This repository currently contains a clean starter project and project instructions for Hermes Agent. The actual gameplay, visual direction, and 2D/3D format have not yet been established in the repository.

## Requirements

- Godot Engine 4.x
- Git

Use the Godot version selected for the project when one is established. Avoid opening and resaving the project in an older or incompatible engine version.

## Open the project

1. Clone this repository.
2. Open Godot Project Manager.
3. Choose **Import** and select the repository folder (the folder containing `project.godot`).
4. Open the project and press **F6** to run the current scene, or **F5** to run the project.

You can also launch it from a terminal:

```sh
godot --path .
```

Headless startup check:

```sh
godot --headless --path . --editor --quit
godot --headless --path . --quit
```

## Working with Hermes Agent

Hermes Agent reads project instructions from `.hermes.md` (highest priority) and supports `AGENTS.md` as a portable project instruction file. Start Hermes from the repository root so it discovers the project context:

```sh
cd /path/to/ebonefire-
hermes
```

Example task:

```text
Inspect the current Godot project, explain its structure, run the available headless checks, and report errors before changing anything.
```

The project instructions ask the agent to inspect before editing, preserve existing work, avoid inventing game design, and verify changes with Godot when available.

Official Hermes documentation: https://hermes-agent.nousresearch.com/docs/user-guide/features/context-files/

## Repository layout

```text
.
├── .hermes.md       # Hermes-specific project instructions
├── AGENTS.md        # Portable coding-agent instructions
├── project.godot    # Godot project configuration
├── scenes/
│   └── main.tscn    # Initial launch scene
├── scripts/
│   └── main.gd      # Minimal startup script
├── assets/          # Add game assets here
├── resources/       # Add reusable Godot resources here
└── docs/            # Design and technical documentation
```

## Current status

- [x] Godot 4 project configuration
- [x] Minimal main scene and startup script
- [x] Hermes Agent project context
- [ ] Confirm whether the game is 2D or 3D
- [ ] Define the core gameplay loop and controls
- [ ] Add original game assets and content
- [ ] Establish automated tests and export targets

**Important:** this scaffold makes the repository recognizable as a Godot project; it does not mean the game itself is implemented or release-ready.
