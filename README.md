![Descent into Madness banner](https://img.itch.zone/aW1nLzE1NjAzNDQxLnBuZw==/original/BPUdiw.png)

# Descent into Madness

A 2D top-down pixel-art roguelike shooter built in Unity. Fight through five levels of procedurally generated dungeons, manage your ammo and sanity, and clear each boss room to descend deeper. Built as a university group game-development project and published as a playable WebGL demo (v1.0.2).

> Status: prototype / demo. It is feature-rich and playable end to end, but it is a student project and not a finished commercial release.

## Play it

**[Play in your browser on itch.io](https://markyu615.itch.io/descent-into-madness)**

No install required. Runs directly in Chrome, Firefox, Safari, or Edge.

```text
https://markyu615.itch.io/descent-into-madness
```

## Tech

- **Engine:** Unity `2022.3.9f1` (LTS)
- **Language:** C# (~150 scripts under `Assets/_Resources/_Scripts`)
- **Rendering:** Universal Render Pipeline (URP) with 2D lighting and post-processing
- **Editor / IDE:** Visual Studio 2022
- **Target:** WebGL (playable build) and Windows standalone

## Features

- **Procedural dungeons:** levels 1–5 are assembled at runtime from room templates (chest, hallway, small, medium, large), so every run is different.
- **Top-down twin-style combat:** WASD movement with mouse aim and point-and-shoot firing.
- **Sanity mechanic:** taking damage briefly triggers a hallucination filter over the screen.
- **In-game minimap:** hold `TAB` (when no enemies are nearby) to open the map UI and click an explored area to fast-travel.
- **Enemy AI:** A* pathfinding plus line-of-sight aiming (enemies and bosses hold fire until they can see you).
- **Boss rooms:** each level ends in a boss room that unlocks after the other rooms are cleared. Beat it to descend.
- **Scaling difficulty:** enemy speed, fire rate, and spawn counts ramp up on each level.
- **Loot and chests:** open chests with `E` for randomized drops (ammo, health, new weapons, or nothing).
- **Multiple weapons:** firearms vary by fire rate, magazine size, reload time, and projectile pattern (bullet, laser, rocket, shotgun).
- **Three playable classes:** the Detective, the Engineer, and the Chad, each with different stats.
- **Interactive environment:** breakable vases and barrels, flippable tables (`E`) that block enemy projectiles, and other damageable props.
- **Audio system:** a 2D sound manager with UI sliders for BGM and SFX volume.
- **Full UI suite:** main menu, instructions, level select, character select, pause, leaderboard / high scores, and a player HUD.
- **Game manager:** tracks run start, win/lose, score, and a hit-combo multiplier.

## Screenshots

No standalone screenshots are committed to this repository yet. For live gameplay and screenshots, see the itch.io page:
**https://markyu615.itch.io/descent-into-madness**

## How to play

| Input | Action |
| --- | --- |
| `W` / `A` / `S` / `D` | Move up / left / down / right |
| Mouse move | Aim |
| Left click / hold | Shoot once / shoot rapidly |
| `R` | Reload |
| `E` | Open chests, flip tables |
| `Space` or `Shift` + `WASD` | Dodge roll in that direction (needs space to roll) |
| `Num 1`–`9` | Switch between picked-up weapons |
| `TAB` | Open the map (only when the room has no enemies) |
| `ESC` | Pause (only when the room has no enemies) |

**Tips**

- You are invincible to enemy damage while rolling, but you cannot shoot or reload mid-roll.
- Use the minimap to fast-travel between cleared rooms.

## Run / open locally

This is a Unity project. The fastest way to play is the [itch.io build](https://markyu615.itch.io/descent-into-madness); to work with the source, open it in the matching Unity version.

**Open in Unity (recommended for development)**

1. Install Unity Hub and **Unity `2022.3.9f1`** (the exact version in `ProjectSettings/ProjectVersion.txt`). The URP and 2D features expect this LTS line.
2. Clone the repo:
   ```bash
   git clone https://github.com/zhenxiao-yu/Descent-In-To-Madness.git
   ```
3. In Unity Hub, choose **Add → Add project from disk** and select the cloned folder.
4. Open the project, then load a scene from `Assets/_Scenes` (start with `MainMenuScene`) and press **Play**.

**Run the prebuilt Windows binary**

A WebGL build is included in `Final-Build-WEBGL/` (and as `Final-Build-WEBGL.zip`). For a Windows desktop build, build from Unity via **File → Build Settings → Windows**, then launch the generated `.exe`.

## System requirements

These reflect the desktop build target.

**Minimum**

- OS: Windows 7 / 8 / 10 (64-bit)
- CPU: Intel Core i3 or equivalent
- RAM: 4 GB
- GPU: NVIDIA GeForce GTX 660 or equivalent
- Storage: 2 GB

**Recommended**

- OS: Windows 10 (64-bit)
- CPU: Intel Core i5 or equivalent
- RAM: 8 GB
- GPU: NVIDIA GeForce GTX 960 or equivalent
- Storage: 2 GB

## Team

A University of Western Ontario group project:

- Mahira Moftah
- Dana Al-kwifi
- Madeline Veysey
- ZhenXiao Yu (Mark Yu)

## License

The original source code in this repository is released under the [MIT License](LICENSE). Copyright (c) 2024 Mark Yu (ZhenXiao Yu).

### Assets

This project uses third-party art, audio, UI, and template assets from the Unity Asset Store and other creators. Those assets are **not** covered by the MIT license above and remain the property of their respective authors under their own terms. The MIT license applies only to the original game code written for this project. If you reuse this repository, you are responsible for sourcing or licensing the third-party assets yourself.

Assets and learning resources used include:

- Pixel Mobs — https://assetstore.unity.com/packages/2d/characters/pixel-mobs-54995
- Pixel UI — https://assetstore.unity.com/packages/2d/gui/pixel-ui-128440
- Pixel Font — https://assetstore.unity.com/publishers/39602
- 2D Simple UI Pack — https://assetstore.unity.com/publishers/34878
- Pixel Art Top Down — https://assetstore.unity.com/packages/2d/environments/pixel-art-top-down-basic-187605
- 2D Roguelike Dungeon Shooter (Rob Ager course) — https://www.udemy.com/course/unity-2d-dungeon-gunner-roguelike-development-course
- Stylized PBR Texture — https://assetstore.unity.com/publishers/52097
- Pixel Monster Pack — https://assetstore.unity.com/publishers/20489
- Pixel Adventure 2 — https://assetstore.unity.com/publishers/44925
- Top Down Adventure Assets — https://assetstore.unity.com/publishers/18720
- Top-down Shooter Engine — https://assetstore.unity.com/packages/templates/systems/tse-2d-topdown-shooter-engine-108589
- Platformer Tileset — https://assetstore.unity.com/publishers/67119
- 2D Pixel Gun Weapon Pack — https://assetstore.unity.com/packages/templates/packs/2d-pixel-gun-weapon-pack-168606
- Particle Pack — https://assetstore.unity.com/packages/vfx/particles/particle-pack-127325
- Pixel Heroes Editor — https://assetstore.unity.com/packages/2d/characters/pixel-heroes-editor-250116
