# Roblox Studio Architect Pro — Claude Skill

[![Claude Skill](https://img.shields.io/badge/Claude-Skill%20%2F%20Plugin-blueviolet.svg)](https://claude.ai)
[![Roblox Studio](https://img.shields.io/badge/Roblox%20Studio-MCP%20Ready-00A2FF.svg)](https://create.roblox.com)
[![Luau](https://img.shields.io/badge/Language-Luau%20Strict-232F3E.svg)](https://luau-lang.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

A production-grade **Claude Skill (`SKILL.md`)** engineered specifically for **Roblox Studio MCP (Model Context Protocol)** workflows. It enforces strict modern Luau engineering, non-destructive (additive) 3D map and level design, token-efficient MCP execution, and responsive UI/UX standards.

---

## Key Features

- **Non-Destructive (Additive) Building:** Never deletes or overwrites previous builds. If you build a farm and later ask to add a barn, Claude inspects existing bounding boxes and expands the map seamlessly alongside your existing structures.
- **Zero-Box Architectural Level Design:** Enforces accurate Roblox stud proportions (doorways, stairs, ceiling heights), foundations, corner pillars, pitched roofs, framed windows, three-tone material harmony, and `PrimaryPart` assignments.
- **Strict Modern Luau Architecture:** Enforces `--!strict`, `task.*` library, `game:GetService()`, `CollectionService` tag-driven systems, server-authoritative exploit protection, `pcall` DataStore resilience, and leak-free connection cleanup.
- **Token-Optimized MCP Workflows:** Prevents recursive full-workspace dumps, encourages batched construction, and avoids echoing entire scripts unnecessarily.
- **Responsive UI/UX Standards:** Enforces `Scale`-based responsive layouts, `UICorner`, `UIStroke`, `UIListLayout`, and `TweenService` micro-interactions.

---

## Prerequisites

To let Claude directly read and edit your Roblox Studio place, make sure you have a **Roblox Studio MCP Server** connected to Claude Desktop or Claude Code (for example, Roblox's official `studio-rust-mcp-server` or a community Roblox Studio MCP bridge).

---

## How to Install & Use

### Method 1: Upload to Claude (Plugins / Skills UI) — Recommended
1. Download the `.zip` archive from the repository releases (or click **Code -> Download ZIP**).
2. Open **Claude** (Desktop or Web) and navigate to **Plugins** -> **Upload a plugin**.
3. Upload the `.zip` file directly (or extract it and upload `SKILL.md`).
4. Click **Upload** to enable the skill in your workspace.

### Method 2: Use with Claude Code (CLI / Local Project)
1. Clone or download this repository.
2. Copy `SKILL.md` into your local Roblox / Rojo project:
   - **As a project skill:** `.claude/skills/roblox-studio-architect-pro/SKILL.md`
   - **Or as root instructions:** rename `SKILL.md` to `CLAUDE.md` in your project root folder.
3. Launch `claude` inside your project directory—the ruleset loads automatically.

---

## Repository Structure

```text
roblox-studio-architect-pro/
├── SKILL.md      # Main Claude Skill with valid YAML frontmatter & full ruleset
├── README.md     # Documentation & step-by-step installation guide
└── LICENSE       # MIT License
```

---

## Example Prompts

Once installed and connected to Roblox Studio via MCP, try prompts like:

- *"Inspect `Workspace/Map/Structures`, then build a rustic wooden barn with a stone foundation, pitched roof, interior hay bales, and warm lighting next to the existing farm."*
- *"Create a server-authoritative `CollectionService` door system for all models tagged `InteractableDoor` with `ProximityPrompt` and smooth `TweenService` hinges."*
- *"Add a responsive bottom-right inventory HUD using Scale, UICorner, and UIStroke without modifying my existing combat scripts."*

---

## License

This project is licensed under the [MIT License](LICENSE).
