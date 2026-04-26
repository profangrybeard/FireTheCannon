# Fire the Cannons!

**GAME 266 — Core Principles: Game Tech · Professor Lindsey · SCAD Atlanta**

A first-Blueprint minigame built in **Unreal Engine 5.6.1**. Students fire a
cannon at destructible walls, learning the full Blueprint pipeline along the
way — components, Enhanced Input, projectiles, collision, Timelines, Chaos
destruction, and basic polish (VFX / audio / camera shake).

> *Our Business is Fun.*

---

## Build Guide

Read it here: **https://profangrybeard.github.io/FireTheCannon/**

The v1.2 guide includes checkboxes, screenshot prompts, progress saving, and
bonus phases.

**Structure of the guide:**

| Session   | Phases  | Topic                                          |
|-----------|---------|------------------------------------------------|
| Monday    | 1 – 6   | Project setup → first shot                     |
| Wednesday | 7 – 11  | Impact, animation, Chaos destruction, polish   |
| Bonus     | B1 – B4 | Charge shots, ammo inheritance, score HUD, slo-mo |

---

## Project Layout

```
FireTheCannons.uproject     Unreal 5.6 project (Blueprint-only)
Config/                     Default .ini files
Content/
├── Blueprints/             Cannon, CannonBall, Wall (+ _Demo variants), M_Landscape
├── BlueprintLibrary_Weapon/  BPFunctionLibrary_Weapon
├── INterfaces/             DamageMultiplier interface
├── Levels/                 L_FireTheCannons, _Damage, _Demo
├── Meshes/                 SM_Cannon, SM_CannonBall, SM_Wall (+ _Demo)
├── Sounds/                 powerful-cannon-shot-352459 (mp3 + uasset)
└── StarterContent/         Standard UE starter pack
index.html                  Build guide (also served via GitHub Pages)
```

---

## Assets

### Blueprints
- **BP_Cannon** / **BP_Cannon_Demo** — player-controlled cannon actor
- **BP_CannonBall** / **BP_CannonBall_Demo** — projectile with damage logic
- **BP_Wall** / **BP_Wall_Demo** — destructible target

### Blueprint Function Library
- **BPFunctionLibrary_Weapon** — shared weapon helpers

### Interfaces
- **DamageMultiplier** — applied by projectiles to deal scaled damage

### Levels
- **L_FireTheCannons** — main playable level
- **L_FireTheCannons_Damage** — damage / destruction sandbox
- **L_FireTheCannons_Demo** — demo / showcase level

### Static Meshes
- **SM_Cannon**, **SM_CannonBall**, **SM_Wall**, **SM_Wall_Demo**

### Materials
- **M_Landscape** — ground material

### Audio
- **powerful-cannon-shot-352459** — cannon fire SFX (mp3 source + imported uasset)

### Starter Content
The standard Unreal starter pack lives in `Content/StarterContent/` — use it
freely for prototyping, but final submissions should rely on your own assets
where possible.

---

## Requirements

- **Unreal Engine 5.6.1** (older versions render Enhanced Input differently
  and the screenshots in the guide will not match)
- Windows or macOS — the guide assumes the Third Person Blueprint template
  with **Starter Content: ON** and **Raytracing: OFF**

---

## License

[MIT](LICENSE) © 2026 profangrybeard
