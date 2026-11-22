<p align="center">
  <img src="assets/banner.png" alt="3D-ARENA Banner" width="100%">
</p>

# ◈ Eclipse Sanctum — 3D Fantasy Boss Rush

[![CI](https://github.com/ISBANDURAHUMAN-R/3D-ARENA/actions/workflows/ci.yml/badge.svg)](https://github.com/ISBANDURAHUMAN-R/3D-ARENA/actions/workflows/ci.yml)

## ◆ About the Project
Eclipse Sanctum is a real-time third-person 3D action boss rush game built entirely within the browser using Three.js and WebGL. Players control an armored knight atop a suspended gothic arena beneath an eclipse, engaging in combat encounters against three multi-phase boss adversaries.

## ❖ Key Features
- Procedural 3D character and creature models constructed with articulated procedural skeletal animation.
- Souls-like action combat engine featuring 3-hit combos, charged heavy attacks, directional dodge rolls with invulnerability frames, timed parries, and spellcasting.
- Three unique boss encounters with distinct attack telegraphs, weak points, and second-phase transformations.
- 100% procedural sound synthesis engine built with the Web Audio API for metal impacts, dragon roars, and ambient atmospheric effects.
- Dual input control scheme supporting keyboard/mouse controls and a mobile touchscreen virtual analog stick.

## ◆ System Architecture
```mermaid
graph TD
    subgraph CoreLoop ["&nbsp; RequestAnimationFrame Engine (60 FPS) &nbsp;"]
        Clock["&nbsp; Three.js Clock / &nbsp;<br/>&nbsp; DeltaTime &nbsp;"] --> Update["&nbsp; Update &nbsp;<br/>&nbsp; Subsystems &nbsp;"]
        Update --> Render["&nbsp; WebGLRenderer &nbsp;<br/>&nbsp; Pass &nbsp;"]
    end

    subgraph InputState ["&nbsp; Dual Input Manager &nbsp;"]
        Keyb["&nbsp; Keyboard &amp; &nbsp;<br/>&nbsp; Mouse &nbsp;"] --> InputBus["&nbsp; Input Action &nbsp;<br/>&nbsp; State &nbsp;"]
        Touch["&nbsp; Virtual Touch &nbsp;<br/>&nbsp; Stick &nbsp;"] --> InputBus
        InputBus --> CombatSM["&nbsp; Combat State Machine &nbsp;<br/>&nbsp; Combo • Roll &nbsp;<br/>&nbsp; Parry • Cast &nbsp;"]
    end

    subgraph WorldScene ["&nbsp; Three.js Scene Graph &nbsp;"]
        Scene["&nbsp; Scene Root &nbsp;"] --> Arena["&nbsp; Suspended &nbsp;<br/>&nbsp; Gothic Arena &nbsp;"]
        Scene --> Knight["&nbsp; Player Model &amp; &nbsp;<br/>&nbsp; Skeleton &nbsp;"]
        Scene --> Bosses["&nbsp; Boss Multi-Phase &nbsp;<br/>&nbsp; Controllers &nbsp;"]
        Scene --> FX["&nbsp; Particle Systems &nbsp;<br/>&nbsp; &amp; Lighting &nbsp;"]
    end

    subgraph AudioEngine ["&nbsp; Procedural Web Audio API &nbsp;"]
        CombatSM --> Synth["&nbsp; Oscillator &amp; &nbsp;<br/>&nbsp; Noise Synth &nbsp;"]
        Bosses --> Synth
        Synth --> Gain["&nbsp; Gain &amp; &nbsp;<br/>&nbsp; Reverb &nbsp;"]
        Gain --> Destination["&nbsp; Audio Output &nbsp;<br/>&nbsp; Destination &nbsp;"]
    end

    CombatSM --> Knight
    Update --> CombatSM
    Update --> Bosses
    Update --> FX
```

## ⬢ Technologies Used
- Three.js (r128)
- WebGL & GLSL Shaders
- HTML5 Canvas
- Tailwind CSS
- Web Audio API

## § Requirements
- Modern web browser with WebGL support

## ▲ Installation & Execution
```bash
# Serve locally using Python
python -m http.server 3000

# Or serve using Node.js
npx serve .
```
Open `http://localhost:3000` in your web browser.

## ※ Developer
Developer: ISBANDU RAHUMAN R  
GitHub: https://github.com/ISBANDURAHUMAN-R
