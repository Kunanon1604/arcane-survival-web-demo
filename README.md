# Arcane Survival — Web Demo

A 2D survivor-like game built with **Godot 4.7.2**, **Claude Code**, and **Godot Editor MCP** as part of a hands-on experiment on [Devlycan](https://devlycan.com). Move to avoid waves of enemies while your weapons attack automatically, collect XP, level up, and try to survive for 5 minutes.

![Arcane Survival running in a browser, showing the HUD, Golems, XP gems, and the survival timer](https://api-tools.devlycan.com/storage/uploads/kSbtR9I9g7_1794797593.webp)

## Read the Article

The full step-by-step experiment, including the prompts, QA results, and performance benchmarks:

- English: [Build a 2D Survivor Game with Claude Code and Godot MCP](https://devlycan.com/blog/build-2d-survivor-game-claude-code-godot-mcp)
- ภาษาไทย: [ทดลองสร้างเกม 2D แนว Survivor-like ด้วย Claude Code และ Godot MCP](https://devlycan.com/th/blog/build-2d-survivor-game-claude-code-godot-mcp)

## How to Play

1. Download `arcane-survival-web-demo.zip` from the [latest release](../../releases/latest).
2. Extract the ZIP file to a folder of your choice.
3. Open a terminal (PowerShell on Windows) in the extracted folder, which contains `index.html`, and run:

   ```bash
   python -m http.server 8000
   ```

   Python is required. If it is not installed, download it from [python.org](https://www.python.org/downloads/).

4. Open `http://localhost:8000` in Chrome or Firefox.
5. When you are done, press `Ctrl+C` in the terminal to stop the server.

> **Note:** Double-clicking `index.html` will not open the game, because browsers do not allow game files to be loaded from your computer without a web server.

## Controls

| Action | Input |
| --- | --- |
| Move | `WASD` or arrow keys |
| Attack | Automatic |
| Upgrade | Choose 1 of 3 options when you level up |

## Features

- 8-directional movement with a smooth following camera
- 3 weapons: Magic Bolt, Orbiting Blades, and Area Pulse
- 3 enemy types: Basic, Fast, and Tank
- XP collection, Level Up, and upgrades for Damage, Cooldown, and Range
- Victory after surviving 5 minutes, and Game Over when HP reaches zero
- Pixel art visuals from the Voxel Dungeon asset pack

## Known Limitations

This game is the result of an experiment and is not a finished product.

- The HUD can be obscured when many Golems are on screen.
- Game balance has not been fine-tuned.
- The game has been tested on desktop browsers only, not on mobile devices.

## Built With

- [Godot Engine 4.7.2](https://godotengine.org/) — Compatibility renderer, single-threaded web export
- [Claude Code](https://code.claude.com/docs/en/overview) — AI coding agent
- [Godot Editor MCP](https://github.com/hybridindie/godot-mcp) — MCP server and add-on connecting Claude Code to the Godot Editor

## Credits

- **Art:** [Voxel Dungeon Sprites & Tiles](https://colefoster.itch.io/voxel-dungeon-pack) by Cole Foster, released under [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/)
- **Experiment and article:** [Devlycan](https://devlycan.com)

## Disclaimer

The term "survivor-like" describes the gameplay style only. This project does not use any characters, artwork, sounds, or assets from Vampire Survivors and has no official affiliation with its developer.
