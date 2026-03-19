#  Better FF Sounds

### A sound replacement mod for Resident Evil: Requiem
<img width="1000" height="547" alt="logo" src="https://github.com/user-attachments/assets/9dcbd04d-b86c-4ae6-a7e5-5cd7d048ae06" />

---

## About

**Better FF Sounds** is a modification for *Resident Evil: Requiem* that gives you full control over the game's audio. Replace any sound in the game with ready-made presets sourced from iconic titles — or craft your own custom sound packs from scratch.

---

## 🎮 Included Presets

| Preset | Source Game |
|---|---|
| `half-life` | Half-Life 2 |
| `cs2` | Counter-Strike 2 |
| `warhammer` | Warhammer 40,000 |
| *...and more* | |

---

## Installation

1. Download the latest release from [Releases](https://github.com/FomaNory/Better-FF-Sounds/releases/tag/release)
2. Launch the mod configurator or edit `config.yaml`
3. Select a preset or point to your custom sound pack
4. Start the game

---

## Custom Sound Packs

Create your own sound replacements in a few simple steps:

```
/sounds/custom/my-pack/
    ├── weapons/
    ├── ambient/
    ├── ui/
    ├── enemies/
    └── pack.yaml
```

Define your pack in `pack.yaml`:

```yaml
name: "My Sound Pack"
author: "YourName"
version: 1.0

replacements:
  pistol_fire: "weapons/my_pistol.ogg"
  reload: "weapons/my_reload.ogg"
  menu_click: "ui/click.ogg"
```

Any sound not specified in your pack will fall back to the currently selected preset or the game's defaults.

---

## Configuration

All settings live in `config.yaml`:

```yaml
# Active sound preset (or path to custom pack)
preset: "cs2"

# Master volume multiplier for replaced sounds
volume: 1.0

# Fall back to original sounds for missing entries
fallback: true
```

