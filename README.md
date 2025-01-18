# IceWall Basic Game

This repository contains a simple Roblox game script that demonstrates the movement mechanics of ice walls. The ice walls move simultaneously between two predefined points (top and bottom) at different speeds while maintaining their orientation. It serves as a beginner-friendly example to learn Roblox scripting concepts, including `BodyPosition` and `BodyGyro`.

## Features

- **Multiple Moving Walls:** Three ice walls that move up and down between predefined points.
- **Varying Speeds:** Each wall moves at a unique speed, creating dynamic gameplay mechanics.
- **Stable Orientation:** Walls maintain their upright position using `BodyGyro`.
- **Script Optimization:** Uses tables and loops for clean and maintainable code.

## Getting Started

### Prerequisites

- Roblox Studio installed on your computer.
- Basic understanding of Lua scripting.

### Installation

1. Clone the repository or download the script directly.
2. Open Roblox Studio and create a new project.
3. Insert three "walls" into the Workspace (`Wall1`, `Wall2`, `Wall3`), each containing:
   - A `top` part (to define the top position).
   - A `bottom` part (to define the bottom position).
   - An `iceWall` part (the moving wall).
4. Paste the script into a Script object within the Workspace.

### Script Overview

The script uses a table-driven approach to manage the walls, making it scalable and easy to customize. Each wall is configured with:
- `top` and `bottom` positions to define its movement range.
- `speed` to control how fast it moves.

```lua
local walls = {
    {top = game.Workspace.Wall1.top, bottom = game.Workspace.Wall1.bottom, iceWall = game.Workspace.Wall1.iceWall, speed = 3},
    {top = game.Workspace.Wall2.top, bottom = game.Workspace.Wall2.bottom, iceWall = game.Workspace.Wall2.iceWall, speed = 5},
    {top = game.Workspace.Wall3.top, bottom = game.Workspace.Wall3.bottom, iceWall = game.Workspace.Wall3.iceWall, speed = 2},
}
