# 🐱 우리동네냥이 (Our Neighborhood Cat)

A pixel art narrative game where you play as a cat exploring a cozy village, interacting with its quirky residents and warming up the town — one paw at a time.

> Built as a demo PoC · Single-file HTML5 · No dependencies

---

## 🎮 Demo Overview

You are a mysterious cat who has wandered into a small village. Each day you have **6 AP (Action Points)** to spend visiting buildings, chatting with NPCs, and making choices that affect the village mood.

**Flow:**
```
Title → Intro → Cat Select → Nyang News → Village Map → Building → Action → Result → Next Day → Ending
```

---

## ✨ Features

- **Pixel art aesthetic** — all assets rendered with `image-rendering: pixelated`
- **Korean pixel font** — neodgm embedded directly (no CDN required)
- **7 explorable buildings** — café, bakery, blacksmith, flower shop, village chief's house, general store, and grandma's house
- **3 interactive NPCs** with unique personalities, multi-line dialogue, and action-specific reactions
  - 달님 🌙 — mysterious café owner
  - 뚝이 🍞 — shy baker with a secret
  - 강쇠 🔨 — gruff blacksmith with a soft side
- **4 non-interactive NPCs** with ambient dialogue (tap to advance)
- **AP system** — spend points on actions, run out and the day ends
- **Village temperature meter** — rises as you make residents happier
- **Fade transitions** between all screens (300ms ease)
- **Animated ending screen** — starfield with twinkle animations

---

## 🕹️ How to Play

1. Open `우리동네냥이_demo.html` in any modern browser
2. Tap/click the title screen to start
3. Follow the intro cards to learn the AP system
4. Select your cat (Mochi is available in the demo)
5. Read today's Nyang News, then head to the village map
6. Move your cat by clicking anywhere on the map
7. Approach a building within **60px** to see the entrance prompt
8. Enter, talk to the NPC, and choose your action
9. Spend all 6 AP to advance to the next day and reach the ending

---

## 📁 File Structure

```
/
├── 우리동네냥이_demo.html   # Single-file game (all assets embedded as base64)
├── README.md
│
└── assets/                  # Source assets (not required to run the game)
    ├── bg_title.png
    ├── bg_map.png
    ├── bg_cafe.png
    ├── bg_bakery.png
    ├── bg_smithy.png
    ├── bg_flower_shop.png
    ├── bg_village_chief_house.png
    ├── bg_general_store.png
    ├── bg_old_wise_woman_house.png
    ├── cat_select_mochi.png
    ├── cat_select_nabi.png
    ├── cat_select_gorum.png
    └── neodgm.woff
```

---

## 🛠️ Tech Stack

| Item | Detail |
|------|--------|
| Engine | Vanilla HTML5 / CSS3 / JavaScript |
| Resolution | 844 × 390px (iPhone landscape ratio) |
| Font | [neodgm](https://github.com/neodgm/neodgm) — embedded as base64 woff |
| Assets | All PNG images embedded as base64 (single-file deploy) |
| Dependencies | None |

---

## 🐾 NPC Actions

Each interactive NPC has their own set of actions tied to their story:

| NPC | Action 1 | Action 2 | Cost |
|-----|----------|----------|------|
| 달님 🌙 | 👀 Observe silently | 🍵 Share warm milk | 1 / 2 AP |
| 뚝이 🍞 | 🍞 Eat fresh bread | 💌 Help deliver heart bread | 1 / 2 AP |
| 강쇠 🔨 | 🔥 Watch the fire | 🔨 Watch him work | 1 / 2 AP |

---

## 🎨 Design Tokens

| Token | Value |
|-------|-------|
| Background base | `#A8C5A0` sage green |
| UI box | `#F5ECD7` cream beige |
| Button | `#8B6F47` warm brown |
| Accent | `#E8956D` warm orange |
| Text | `#3D2B1F` dark brown |
| Dialog overlay | `rgba(30,20,10,0.82)` |

---

## 📌 Known Limitations (Demo Scope)

- Only Mochi is selectable (Nabi & Gorum are locked — "coming soon")
- Non-interactive NPCs have ambient dialogue only (no action system)
- Village temperature and AP stats are partially dummy values
- No save/load — demo runs as a single session

---

## 📝 License

This project was created as a game demo PoC.
Assets and font are for demo purposes only.

---

*🐱 우리동네냥이 — Made with pixels and purrs*
