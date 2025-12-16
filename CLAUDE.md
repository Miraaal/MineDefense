# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**MineDefense** is a hybrid maze exploration + tower defense game prototype being developed as a portfolio project by a 2-person team. The core gameplay loop involves simultaneous multitasking:
- **Left hand (keyboard)**: Navigate maze with arrow keys and mine resources
- **Right hand (mouse)**: Place towers/barricades to defend against monsters

This is an early-stage prototype focusing on core mechanics before detailed balancing and UI work.

## Development Environment

- **Unity Version**: 6000.2.8f1 (Unity 6)
- **Render Pipeline**: Universal Render Pipeline (URP)
- **Input System**: New Unity Input System (version 1.14.2)
- **Key Packages**:
  - `com.unity.ai.navigation` (2.0.9) - For pathfinding
  - `com.unity.inputsystem` (1.14.2) - For input handling
  - `com.unity.render-pipelines.universal` (17.2.0) - URP rendering

## Core Systems to Implement

The prototype aims to implement these 5 core systems (currently in planning/early development):

1. **Procedural Maze Generation**: Generate maze maps procedurally
2. **Monster AI**: Monster spawning and pathfinding (likely A* algorithm)
3. **Tower System**: Tower placement and automatic attack mechanics
4. **Barricade System**: Placeable obstacles that block monster movement
5. **Player Movement**: Keyboard-based movement controls

## Git Workflow

**IMPORTANT**: When committing code changes, always update `박진석_개발일지.md`:

1. Commit your code changes first
2. Update `박진석_개발일지.md` with today's date (`## YYYY-MM-DD`) and a brief bullet list of what was done
3. Commit the updated development log
4. Push both commits together

Example development log entry:
```markdown
## 2025-12-16

- Unity 프로젝트 생성 (URP)
- Git 저장소 초기화 및 GitHub 연동
```

Keep entries concise - just bullet points of completed work.

## Project Structure

```
Assets/
├── Scenes/          # Game scenes
├── Scripts/         # All C# game scripts (currently minimal)
└── Settings/        # URP and rendering configuration
```

All game code goes in `Assets/Scripts/`. Currently contains only a placeholder `Test.cs`.

## Architecture Notes

- This is a greenfield Unity 6 project - architecture patterns are not yet established
- Team is in the planning phase; detailed system design will emerge during prototype development
- Focus is on getting core mechanics working before optimization or architectural refinement
