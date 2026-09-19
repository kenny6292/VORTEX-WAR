# UNREAL ENGINE 5 INTEGRATION

Unreal Engine 5 handles real-time 3D gameplay: world simulation, movement, shooting, physics, vehicles, aircraft, watercraft, animation, audio, VFX and authoritative dedicated-server simulation.

The web/game-services platform provides authentication, profiles, inventory, loadouts, matchmaking, progression, ranks, social, tournaments and economy services.

Architecture:
Player Client → Authentication → Matchmaking → Dedicated Authoritative Server → Game Services → PostgreSQL/Supabase

Clients must never be authoritative for damage, health, inventory ownership, currency, XP, rank or match results.
