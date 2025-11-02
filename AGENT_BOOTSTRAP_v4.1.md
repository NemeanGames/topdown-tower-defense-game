# AGENT_BOOTSTRAP_v4.1
This orchestrator defines eight packets for a top-down tower defense shooter webapp game. The orchestrator will spawn parallel agents to handle each aspect of development. Each agent must produce a plan, code, test, and commit for its tasks. The aggregator will merge passing packets and deploy to GitHub Pages or Vercel.

## Packets

### Design
- Define gameplay loop: Build phase (place towers on editable tiles) and Combat phase (player controlling top-down shooter).
- Define tower types, enemy types, pathing rules (A* dynamic path).
- Create UI/UX flow for grid maps, turret placement, player controls.
- Document towers, weapons, equipment, perks, waves.

### Data
- Define JSON schemas for tile maps, weapon configs, tower stats, enemy stats.
- Provide example tile map with fixed walls, open tiles, core tile.
- Provide weapon config JSON with damage, rpm, mag size, reload, spread, projectile speed.
- Provide upgrade and perk tables.

### Core
- Implement game engine: grid map representation, A* pathfinding with dynamic updates.
- Implement tower mechanics: target, shoot, damage.
- Implement top-down shooter controls: WASD movement, mouse aim, shooting, reload, weapon switching, equipment usage.
- Implement waves and enemy AI: path to core, dynamic aggro between player and core.

### UI
- Implement canvas-based rendering for grid, towers, enemies, player.
- Implement HUD: health, armor, ammo counters, equipment icons, perk slots.
- Implement build-phase overlay for tower placement, invalid placement indicator.
- Implement mini-map and wave timers.

### Economy
- Implement currency for buying/upgrading towers and weapons.
- Define XP system for unlocking perks and equipment.
- Adjust rewards based on path length and difficulty.

### State
- Implement save/load for maps, player stats, unlocked perks.
- Implement browser persistence (localStorage).

### QA
- Write unit tests for pathfinding, tower targeting, shooter mechanics.
- Provide debug overlay.

### Deploy
- Provide build pipeline using bundler (e.g., Vite).
- Configure GitHub Pages deployment with fallback to Vercel.
- Update README with instructions to run and build.

## Execution
Start the orchestrator by running the v4.1 Orchestrator Start prompt with 8 parallel packets. Agents should self-organize and report via aggregator.
