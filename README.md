# Dungeon RPG V2.0

2D top-down dungeon RPG made with Godot 4.7.2 (THE HOLLOW / 地城試煉).
A chibi warrior descends 30 dungeon floors, collects gear, grows a build and defeats the Final Boss.

**Play in the browser (GitHub Pages):** the web build is in `docs/`.
Once Pages is enabled, open `https://xxsunxxsun.github.io/dungeon-rpg/`.
No EXE download and no Godot install are needed.

## Content

- **30-floor dungeon**, 10 regions: Moss, Ember, Ruins, Swamp, Frost, Lava, Abyss, Tomb, Void and Demon Castle. Linear main path with side branches, plus special rooms, secret rooms, traps and events.
- **Many monster types (43)**: active aggro and group alerts, ranged attacks, keeping distance, dashes, summons, blinks, self-destructs and status effects. **Split monsters** break into smaller copies when killed.
- **Elite** monsters with random abilities that guard treasure chests.
- **Bosses (12)**: multi-phase, with enrage. Floor 30 holds the **Final Boss** (3 phases: melee, projectiles, AOE, summons, status, blinks, ground skills, enrage).
- **Monster skills**: projectiles, warning zones, summons, revives, life drain and more.
- **Player skills**: basic slash, heavy slash, **sword wave** (element depends on the weapon), whirlwind, charged ground slam; MP and cooldowns.
- **Weapons and armor**: 5 slots, 5 rarities (Common / Uncommon / Rare / Epic / Legendary) and affixes.
- **Enhancement** up to +10 and **forging**: dismantle, craft, reforge.
- **Shop**: the female merchant 玲玲. **Blacksmith**: a chibi female blacksmith.
- **GARY Buff**: answer GARY's English questions and tongue twisters at his altar for extra blessings (ATK, HP, LUCK, EXP, SPD, Gold, Skill Damage).
- **Talents and classes**: talent trees, passives, class change and build slots.
- **Hard Mode**, **Boss Rush** and **Endless Dungeon** challenge modes, with challenge records.
- **Achievements** and statistics.
- **Save / Load**: automatic saves. The browser version keeps saves in the browser's local storage (IndexedDB), so they are still there after closing and reopening the page.
- **Backpack**: separate Bag / Equipment / Sell pages; multi-select sell, batch delete, type and rarity filters, item locking.

## Controls

These are read from the game's actual input settings (`scripts/managers/input_bindings.gd` and the HUD).

| Action | Keys |
| --- | --- |
| Move | W A S D / arrow keys |
| Basic attack | Space / left mouse button (aims at the cursor) |
| Heavy slash | 1 / J |
| Sword wave | 2 / K / middle mouse button |
| Whirlwind | 3 / L |
| Charged ground slam | Hold F / right mouse button, release to cast |
| Interact (chest, stairs, shop, forge, GARY) | E |
| Potion | Q |
| Backpack | I / Tab |
| Talents | T |
| Character | C |
| Map | M |
| Pause (settings, achievements) | Esc |
| Replay (on the end screen) | R |
| GARY question answers | A / B / C / D or 1–4 |

Fullscreen: Esc → Settings → Fullscreen. The game never switches to fullscreen on its own when it starts.

### Phone / tablet (touch)

Play in **landscape**. On-screen controls appear automatically on touchscreens:

| Control | Where |
| --- | --- |
| Move | Joystick: drag anywhere on the left side |
| Attack | Big 攻擊 button, bottom right (hold to keep attacking) |
| Interact / Potion | E 互動 and Q 藥水 buttons |
| Skills | Tap the skill slots (bottom right); hold F to charge the ground slam |
| Menus | 背包 / 天賦 / 角色 / 地圖 / 選單 buttons, top right |

Menus, shop, forge and GARY's questions are tapped directly. The first load downloads about 72 MB (cached afterwards).

## Versions

- **Windows**: `Dungeon RPG V2.0`, full-quality settings.
- **Web** (`docs/`): `Dungeon RPG V2.0 Web`. Web Performance Mode automatically lowers caps on crowds, projectiles and effects; gameplay rules are unchanged.

## Publishing (GitHub Pages)

Settings → Pages → Build and deployment → Deploy from a branch → Branch `main`, Folder `/docs` → Save.

`docs/` contains only the Godot Web Export runtime files: `index.html`, `index.js`, `index.wasm`, `index.pck`, icons and audio worklets.

## Art

Characters, monsters, scenes and UI are placeholders for now. The final art will replace them later.
