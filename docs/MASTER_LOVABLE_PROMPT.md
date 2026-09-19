# VORTEX WAR — MASTER LOVABLE BUILD PROMPT

Build VORTEX WAR, a premium original multiplayer war-game ecosystem with the tagline ENTER THE BATTLEFIELD. Build the complete responsive website, player platform, admin platform, database and secure game-services integration layer. Do not pretend the browser is the AAA 3D game engine; Unreal Engine 5 and authoritative dedicated servers handle real-time gameplay.

## Brand
Premium, cinematic, futuristic military, tactical, dark, high contrast, metallic and HUD-inspired. Original identity only. Do not copy proprietary characters, maps, logos, UI, artwork, sounds or animations from existing games.

## Website
Create Home, Game, Modes, Operators, Weapons, Vehicles, Maps, Battle Royale, Ranked, Battle Pass, Shop, Tournaments, News, Events, Community, Support, Download/Play entry, legal pages, Login and Registration.

## Player Platform
Authenticated dashboard with profile, inventory, loadouts, operators, weapons, vehicles, cosmetics, missions, achievements, XP, rank, match history, leaderboards, Battle Pass, VORTEX Credits, shop, friends, messages, notifications and settings.

## Operators
Support 85 total: M-01–M-50 male, F-01–F-20 female, S-01–S-15 specialists. Each has unique ID, name, role, faction, lore, biography, ability/perk, difficulty, rarity, outfit, skins, statistics and progression. Roles include Assault, Recon, Support, Defender, Medic, Scout, Engineer, Tactical, Heavy and Specialist. No pay-to-win abilities.

## Weapons
Support 110+ original weapons: 25+ AR, 15+ SMG, 12+ shotgun, 12+ sniper, 10+ marksman, 12+ LMG, 12+ pistol, 6+ launcher, 6+ melee. Support optics, muzzles, barrels, grips, magazines, stocks, lasers, ammunition and underbarrel attachments. Track stats, progression, skins and unlocks.

## Vehicles
32 ground vehicles; 12 aircraft; 8 watercraft. Track speed, armor/health, handling, seats/capacity, damage, rarity, skins and unlocks. Unreal handles physics and simulation.

## Battle Royale
Support Solo, Duo and Squad with 20–50 players per match. Architecture must support 50 from the beginning; test 20 → 30 → 40 → 50. Squad target: 4. Provide lobby, party, ready state, matchmaking, match state, results, XP and history.

## Battle Royale Maps
1. Vortex Island
2. Iron Desert
3. Neon City
4. Frostline
5. Black Haven
6. Storm Valley
7. Red Canyon
8. Ashfall
9. Titan Coast
10. Verdant Wilds
11. Dead Frontier
12. Skyline Province
13. Crimson Highlands
14. Omega Territory
15. Eclipse Archipelago

## Multiplayer
Target 22 multiplayer maps. Modes: Team Deathmatch 10v10, Domination 10v10, Search & Destroy, Free-for-All, Ranked, Custom Match, Training Ground, Vortex Arena and Tournament Mode.

## Matchmaking / Parties
Create casual/ranked matchmaking architecture, region and ping metadata, party queues, invitations, ready state and server allocation hooks. Do not display fabricated live-player or matchmaking data.

## Inventory / Loadouts
Inventory categories: operators, skins, weapons, attachments, vehicles, aircraft, watercraft, equipment, emotes, charms, banners, titles and badges. Loadouts include operator, primary, secondary, melee, tactical, lethal, perks and attachments. Ownership is server-authoritative.

## Progression
Player XP, levels, weapon XP, operator progression, unlocks, missions, challenges, achievements and seasonal progression. Rewards can derive from matches, wins, eliminations, missions, events and tournaments.

## Ranked
Bronze, Silver, Gold, Platinum, Diamond, Master, Grandmaster, Vortex Elite. Track rank points, promotion/demotion, seasonal reset, rank history, badges and rewards.

## Battle Pass
Free + Premium tracks, 100+ reward-slot architecture, operator/weapon/vehicle cosmetics, emotes, banners, VORTEX Credits and seasonal rewards. No pay-to-win advantages.

## Economy
Currency: VORTEX CREDITS. Server-side balance and transaction validation. Shop supports operators, cosmetics, weapon skins, vehicle/aircraft/watercraft skins, emotes, charms, banners, titles, bundles and Battle Pass. Never put payment secrets in frontend.

## Tournaments
Discovery, registration, teams, brackets, schedules, match results, leaderboards, rewards, rules and announcements. Design for future esports expansion.

## Social
Friends, requests, online/offline status, recently played, block/report, party invites, player search, direct/squad/lobby/tournament chat and moderation controls.

## News / Events
News, articles, events, seasons, patch notes, featured content and tournament announcements. Admin publishing workflow.

## Admin
Protected RBAC admin console for players, moderation, reports, bans/suspensions, operators, weapons, vehicles, maps, equipment, missions, rewards, cosmetics, shop, Battle Pass, tournaments, news, events, virtual currency, transactions, analytics and audit logs.

## Database
Use Supabase/PostgreSQL with tables: profiles, player_stats, player_ranks, matches, match_players, game_modes, weapons, weapon_attachments, weapon_skins, characters, character_skins, vehicles, vehicle_skins, maps, inventory, inventory_items, loadouts, friends, friend_requests, messages, missions, player_missions, achievements, rewards, battle_pass, battle_pass_rewards, player_battle_pass, shop_items, transactions, virtual_currency, tournaments, tournament_teams, tournament_matches, leaderboards, notifications, news, events, reports, admin_users and audit_logs.

Use foreign keys, indexes, constraints, RLS and secure server-side validation.

## API Contract
POST /auth/session
GET /player/profile
GET /player/inventory
GET /player/loadouts
GET /characters
GET /weapons
POST /matchmaking/queue
GET /matchmaking/status
POST /matches/result
GET /player/stats
GET /player/rank
GET /leaderboards
GET /missions
POST /missions/claim
GET /tournaments
POST /tournaments/join
POST /shop/purchase
GET /news
GET /events

Sensitive actions must be validated server-side.

## Security / Anti-Cheat
Validate movement, fire rate, damage, hits, inventory, currency, XP, rank, rewards and match results server-side. Support telemetry, suspicious-behavior detection, reports, bans/suspensions and audit logs. Unreal dedicated servers remain authoritative for real-time gameplay.

## Unreal Engine Integration
Prepare authentication/token validation, player services, inventory synchronization, loadouts, matchmaking, match creation/status, match results, progression, rewards, social and economy service contracts. Clients submit intent; authoritative servers determine gameplay outcomes.

## Content Scale
Architecture must support 150+ buildings, 500+ environment assets, 500+ props, 150+ equipment items, 300+ cosmetics and 200+ VFX. The web app stores metadata and content references; actual 3D assets belong in the game/content pipeline.

## OmniForge AI Integration
OmniForge AI is a separate general-purpose AI 3D creation platform. VORTEX WAR should support future import metadata: asset ID, type, version, creator, license, polygon count, texture resolution, LODs, skeleton, animation set, engine compatibility and approval status. Do not build OmniForge inside VORTEX WAR.

## UX
Desktop/tablet/mobile responsive. Use cinematic transitions, polished hover states, skeletons, loading, empty/error/success states, toasts and modals. Avoid generic templates, lorem ipsum, dead buttons, fake statistics and insecure client-side state.

## Production Phases
1. Foundation: brand, site, auth, Supabase, database, dashboard, profile.
2. Game content: operators, weapons, vehicles, maps, modes, inventory, loadouts.
3. Progression: XP, missions, achievements, ranked, leaderboards, Battle Pass.
4. Social: friends, parties, messaging, notifications, reports.
5. Economy: VORTEX Credits, shop, transactions, Battle Pass purchases.
6. Competitive: ranked and tournaments.
7. Game integration: Unreal authentication, matchmaking, player services, inventory/progression sync and match results.
8. Live service: seasons, maps, operators, weapons, vehicles, events, cosmetics and tournaments.

## Final requirement
Build a maintainable, secure, scalable foundation for a real multiplayer game. Do not fabricate capabilities that require Unreal/dedicated servers. Implement what the web platform can actually do, and leave clean interfaces for the real-time game layer.
