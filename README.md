# ⚔️ ECLIPSE SANCTUM — 3D Fantasy Boss Rush Action RPG

[![Status](https://img.shields.io/badge/Status-Implementation--Ready-emerald?style=for-the-badge)](https://github.com/)
[![Engine](https://img.shields.io/badge/Engine-Three.js_r128-amber?style=for-the-badge&logo=threedotjs)](https://threejs.org/)
[![Audio](https://img.shields.io/badge/Audio-Web_Audio_API_Synthesizer-purple?style=for-the-badge)](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API)
[![Styling](https://img.shields.io/badge/HUD-Tailwind_CSS-38bdf8?style=for-the-badge&logo=tailwindcss)](https://tailwindcss.com/)
[![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)](LICENSE)

> A high-octane, dark-fantasy 3D Boss Rush Action RPG inspired by *Elden Ring*, *Dark Souls*, and *Monster Hunter*. Built entirely with WebGL, Three.js, and procedural Web Audio. Challenge three legendary Fallen Lords atop a suspended ruined cathedral beneath a cosmic Void Eclipse.

---

## 🌟 Visual & Character Redesign Overhaul

Both the **Hero (Ashen Sovereign)** and **All Three Boss Opponents** have undergone a comprehensive visual and architectural overhaul, replacing generic primitives with ornate, high-fantasy 3D procedural models, anatomical silhouettes, PBR shaders, dynamic emissive glows, and articulated procedural animations:

### 🛡️ The Hero: The Ashen Sovereign (Eclipse Knight)
* **Corinthian Knight Bascinet & Greathelm**: Tapered skull dome with reinforced brow comb, sculpted face mask, glowing horizontal cross-visor slit emitting weapon-aligned energy, flared cheek guards, sweeping dragon winglet fins, and a flowing royal knight plume.
* **Sculpted Cuirass & Sanctum Heart Medallion**: Anatomically curved plate cuirass with angled deflection pectoral plates, gold gorget collar, and a central glowing **Sanctum Sun Medallion** with a pulsing octahedron core that channels cosmic energy.
* **Tiered Spaulders & Articulated Gauntlets**: 3-tiered spiked gothic pauldrons with gold rims and sword-breaker blades, elbow couter spikes, vambraces, and knuckle plates.
* **Faulds & Chainmail Underskirt**: Overlapping hip tassets with golden diamond rivets revealing dark chainmail armor underneath.
* **Articulated Sabatons**: Segmented cuisses with leather strapping, spiked knee poleyns, fluted shin greaves, and pointed gothic sabatons with heel spurs.
* **Dynamic Billowing Cape**: Multi-segment articulated cape that ripples realistically in the cathedral winds during running, dodging, and heavy swings.
* **Ornate Gothic Heater Shield**: Curved steel kite shield featuring an embossed golden eclipse sunburst medallion, glowing rune core, and heraldic cross borders.

---

### 👹 Opponent I: Vaelgor, Colossal Armored Knight (Lord of the Ember Furnace)
* **Towering Demonic Silhouette**: Standing over 6.5 meters tall, encased in blackened furnace plate with gold filigree trims.
* **Horned Executioner Helm**: Menacing iron skull faceplate with a 4-slit magma visor and two massive swept demonic obsidian horns with glowing molten tips.
* **Back Steam-Furnace Engine (Tactical Weakpoint)**: An alchemical steam engine mounted on his upper back featuring three vertical magma fuel canisters encased in iron cages, a glowing power core, and dual angled smoking exhaust chimneys venting molten embers.
* **The World-Breaker Greatsword**: A monstrous 6.2-meter serrated magma slab blade crackling with fiery fuller veins, hooked barb flanges, and a dragon jaw crossguard.
* **Furnace Fortress Greatshield**: Monolithic dark steel tower barrier with an embossed fiery demonic eye that glares at the player and ground-cleaving bottom spikes.

---

### 🔮 Opponent II: Seraphina, Corrupted Celestial Mage (Archon of the Void Eclipse)
* **Celestial Seraph Deity Silhouette**: Gracefully levitating in zero gravity above the cathedral arena, draped in starry cosmic silk gowns with golden filigree hems.
* **Porcelain Mask & Eclipse Tiara**: Sculpted porcelain face with a glowing golden astral blindfold, towering multi-spire eclipse crown, and cascading cosmic hair.
* **Concentric Gyroscopic Eclipse Halo**: Dual counter-rotating astronomical astrolabe rings floating behind her, featuring an inner zodiac ring, glowing starlight nodes, and a central black hole void sphere with a radiant violet corona.
* **6 Crystalline Starlight Wings**: Six tiered articulated wings shaped like arching luminous blades with translucent starlight crystalline membranes that flap and breathe with cosmic harmonics.
* **The Eclipse Astrolabe Staff**: A 5.2-meter catalyst staff crowned with an astronomical gyroscope armillary sphere: three interlocking rotating rings enclosing a blazing pulsar star orb.
* **Orbiting Planetary Satellites**: Three miniature stellar crystals orbiting her body in 3D ellipses.
* **Geodesic Astral Barrier**: Hex-grid geodesic forcefield that hums into existence whenever she channels devastating spells.

---

### 🐉 Opponent III: Malakor, The Shadow Dragon (Sovereign of the Abyssal Tempest)
* **Terrifying Predatory Dragon Anatomy**: Massive muscular quadrupedal/bipedal dragon torso clad in jagged obsidian scales with continuous graduated spinal dorsal plates.
* **Predatory Skull & Articulated Maw**: Elongated skull with brow ridges, glowing predatory slit-pupil crimson eyes, sweeping crown horns, secondary cheek spikes, and an articulated lower jaw lined with razor-sharp white fangs.
* **Internal Throat Flame & Abyssal Heart Core**: An internal throat flame nodule that flares blinding bright during breath attacks, and a pulsating crimson-violet corruption heart core exposed on his chest.
* **Articulated Sweeping Wings**: Anatomical dragon wings with defined shoulder joints, humerus arm bones, apex thumb claws, and four sweeping finger spars supporting translucent dark crimson wing membranes with glowing veins.
* **Razor-Taloned Limbs**: Four muscular dragon legs terminating in heavy paws with curved razor talons gripping the arena stones.
* **7-Segment Serpentine Tail**: Multi-segment articulated tail that propagates organic wave whips, ending in a lethal four-bladed shadowflame mace thagomizer.

---

## 🎮 Combat Codex & Mastery Mechanics

| Action | Keyboard / Mouse / Touch | Description |
| :--- | :--- | :--- |
| **Virtual Joystick** | `Drag Knob` (Bottom-Left) | 360° Analog Thumbstick for smooth robot/warrior movement with touch or mouse |
| **Move** | `W`, `A`, `S`, `D` / Arrows | Omnidirectional locomotion (also dynamically deflects on-screen joystick knob) |
| **Light Attack** | `Left Click` / `J` | Fluid 3-hit weapon combo with scaling poise damage and ribbon trails |
| **Charged Heavy** | `Right Click` (Hold) / `K` | High-damage hyperarmor strike that severely damages enemy posture |
| **Dodge Roll** | `Space` / `Shift` | 0.32s invulnerability frames (i-frames) in movement direction |
| **Perfect Dodge** | `Space` on impact | Triggers slow-mo bullet time, restores stamina, and grants **Counter Surge (+35% damage)** |
| **Parry / Guard** | `Q` / `F` | Timed deflection: nullifies damage and inflicts massive **Posture Break** |
| **Cast Spell** | `E` / `1` | Casts currently equipped Boss Relic spell |
| **Sanctum Flask** | `R` / `2` | Drinks healing draught (restores 45% Max HP, 4 charges per encounter) |
| **Lock-On** | `Tab` / `Middle Click` | Toggles dynamic third-person target tracking reticle |
| **Camera Orbit** | Mouse Drag | Free-look camera control when Lock-On is disabled |
| **Camera Zoom** | `Mouse Wheel` | Smoothly zooms battlefield camera perspective |

---

## 🏆 Boss Roster & Strategy Guide

```
+-----------------------------------------------------------------------------------+
|  LORD I: VAELGOR, COLOSSAL KNIGHT                                                 |
|  HP: 4,200 | Posture: 100 | Phase II: Ember Furnace Lord                          |
|  - Weakness: Timed Parry [Q] on broad cleaves; flank and strike his Back Furnace  |
|    Engine after heavy overhead slams.                                             |
|  - Phase II: Volcanic leap slams that erupt traveling magma waves across floor.   |
+-----------------------------------------------------------------------------------+
|  LORD II: SERAPHINA, CELESTIAL MAGE                                               |
|  HP: 3,800 | Posture: 100 | Phase II: Archon of the Void Eclipse                  |
|  - Weakness: Strike her with a Spell [E] or Charged Heavy while she channels her  |
|    Astral Beam to completely shatter her Astral Barrier and stagger her!          |
|  - Phase II: Rapid gravity blinks, quintuple homing starlight seeker barrages.    |
+-----------------------------------------------------------------------------------+
|  LORD III: MALAKOR, THE SHADOW DRAGON                                             |
|  HP: 5,200 | Posture: 120 | Phase II: Sovereign of Abyssal Tempest                |
|  - Weakness: Avoid lingering behind (tail whip punish); bait breath or skyward    |
|    dive-bomb and punish the exposed chest Abyssal Heart Core for 1.45x criticals. |
|  - Phase II: Skyward dive-bombs with massive crimson ground telegraph impact.    |
+-----------------------------------------------------------------------------------+
```

---

## 🛡️ Relic Armory & Progression System

Defeating each boss permanently forges their essence into weapons, spells, and armor sets:

### 🗡️ Weapons
1. **Sanctum Claymore** *(Default)*: Balanced knightly rune-blade with glowing fuller channel (95 DMG, 18 Poise).
2. **Vaelgor's Ember Greatsword** *(Vaelgor Unlock)*: Massive serrated magma slab sword (145 DMG, 32 Poise, 3.9 Reach).
3. **Seraphina's Starlight Glaive** *(Seraphina Unlock)*: Crystalline poleblade with swift luminous slashes (118 DMG, 22 Poise, 1.22 Speed).
4. **Malakor's Abyssal Fang** *(Malakor Unlock)*: Jagged dragon bone blade pulsing with dark crimson veins (165 DMG, 30 Poise).

### ✨ Spells
1. **Arcane Soul Lance** *(Default)*: High-speed piercing lance of sanctum light (140 DMG, 3.5s CD).
2. **Molten Earthbreaker** *(Vaelgor Unlock)*: Erupts four successive traveling volcanic shockwaves (230 DMG, 5.5s CD).
3. **Celestial Homing Orbs** *(Seraphina Unlock)*: Conjures five starlight orbs that track the target (210 DMG, 4.8s CD).
4. **Abyssal Breath Surge** *(Malakor Unlock)*: Unleashes a wide shadowflame tempest cone (285 DMG, 6.2s CD).

### 🥋 Cosmetic Armor Sets
1. **Silver Sanctum Plate** *(Default)*: Consecrated silver steel with gold filigree and royal blue cape.
2. **Vaelgor Dreadplate** *(Vaelgor Unlock)*: Blackened colossus armor glowing with furnace embers and crimson cape.
3. **Celestial Arch-Vestments** *(Seraphina Unlock)*: Deep violet star-woven battle armor with purple cape.
4. **Abyssal Dragonscale** *(Malakor Unlock)*: Obsidian scales harvested from Malakor with dark maroon cape.

---

## 🚀 How to Run the Project

This project is **100% implementation-ready** and requires zero external build tools, bundles, or heavy asset downloads.

### Option 1: Zero-Install Instant Play (Recommended)
Simply double-click **`index.html`** or **`eclipse_sanctum_3d_boss_rush_action_rpg.html`** to launch the game directly in any modern web browser (Chrome, Edge, Firefox, Safari).

### Option 2: Local Dev Server with Node.js
```bash
# Run with npx serve
npm start
# or
npm run dev
```
Open [http://localhost:3000](http://localhost:3000) in your browser.

### Option 3: Python Built-In Server
```bash
python -m http.server 3000
```
Open [http://localhost:3000](http://localhost:3000) in your browser.

### Option 4: Deploy Anywhere
Simply upload `index.html` to **GitHub Pages**, **Vercel**, **Netlify**, or any static web host.

---

## 🛠️ Architecture & Tech Stack

* **Rendering Engine**: Three.js r128 WebGL with PCFSoftShadowMap, PBR standard materials, and ACESFilmicToneMapping.
* **Audio System**: Procedural Web Audio API synthesizer generating real-time resonant steel clangs, deep impact booms, spell chimes, dragon roars, and healing chimes with zero external audio file latency.
* **Interface & HUD**: Modern Tailwind CSS dark glassmorphism, responsive souls-like health/poise delayed trail bars, combat alert pills, and floating damage numbers.
* **Procedural Assets**: 100% procedural 3D model construction, guaranteeing instantaneous loading without 404 texture or model loading errors.

---

## 📜 License
Distributed under the **MIT License**. Free for personal, academic, and commercial use.
