# VORTEX WAR
## ENTER THE BATTLEFIELD

VORTEX WAR is an original premium multiplayer war-game ecosystem. This repository contains the web platform/game-services foundation and production blueprint. The real-time 3D shooter is intended for Unreal Engine 5 with authoritative dedicated servers.

## Targets
- 85 operators: 50 male, 20 female, 15 specialists
- 110+ weapons
- 32 ground vehicles
- 12 aircraft
- 8 watercraft
- 15 Battle Royale maps
- 22 multiplayer maps
- 20–50 players per Battle Royale match
- 150+ buildings, 500+ environment assets, 500+ props
- 150+ equipment items, 300+ cosmetics, 200+ VFX

## Architecture
Player Client → Auth → Matchmaking → Authoritative Dedicated Server → Game Services → PostgreSQL/Supabase

Lovable/React/TypeScript/Tailwind/Supabase provides the player website and game-services layer. Unreal Engine 5 provides real-time 3D gameplay.

See docs/MASTER_LOVABLE_PROMPT.md for the full build specification.
