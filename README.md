# GALAGA Clone - Classic Arcade Shooter

<div align="center">

![Galaga Screenshot](https://img.shields.io/badge/HTML5-Canvas-orange) ![JavaScript](https://img.shields.io/badge/JavaScript-Pure ES6-yellow) ![No Dependencies](https://img.shields.io/badge/Dependencies-None-green) ![License](https://img.shields.io/badge/License-MIT-blue)

**A faithful recreation of the 1981 Namco classic, built with pure HTML5 Canvas**

[Play Now](https://galaga-clone-mark.netlify.app) | [Report Bug](https://github.com/mark202/galaga-clone/issues)

</div>

---

## 🎮 Game Features

### Core Gameplay
- **Player Ship**: Smooth left/right movement with arrow keys or A/D
- **Shooting**: Rapid-fire with spacebar, shoot down enemies
- **3 Lives System**: Classic arcade lives with invincibility frames on respawn
- **Wave Progression**: Endless waves with increasing difficulty

### Enemy Types

| Enemy | Color | Points | Behavior | Difficulty |
|-------|-------|--------|----------|------------|
| **Bee** | Yellow/Orange | 100 | Fast, basic attack patterns | Easy |
| **Butterfly** | Cyan/Blue | 150 | Medium speed, diving attacks | Medium |
| **Boss** | Magenta | 400 | Large, fierce, multi-directional shots | Hard |

### Visual Effects
- **CRT Scanlines**: Authentic retro arcade monitor effect
- **Screen Glow**: Subtle phosphor glow simulation
- **Star Field**: Parallax scrolling background stars
- **Explosions**: Particle-based explosion animations
- **Engine Thrust**: Animated engine flames on player ship

### Game States
- **Title Screen**: Animated enemy parade, high score display
- **Playing**: Full gameplay with HUD
- **Wave Complete**: Brief intermission between waves
- **Game Over**: Final score display with high score tracking

---

## 🕹️ Controls

| Key | Action |
|-----|--------|
| `←` / `→` or `A` / `D` | Move ship left/right |
| `Space` or `Z` | Fire laser |
| `Enter` or `Space` | Start game / Restart |

---

## 🎯 How to Play

1. Open `index.html` in any modern browser
2. Press **Enter** or **Space** to start
3. Move your ship to dodge enemy bullets
4. Shoot enemies before they destroy you
5. Clear all enemies to advance to the next wave
6. Survive as long as possible and beat your high score!

---

## 🏗️ Technical Implementation

### Pure Vanilla Stack
- **HTML5 Canvas**: Hardware-accelerated 2D rendering
- **ES6 JavaScript**: Modern JS with classes and arrow functions
- **CSS3**: CRT effects using gradients, shadows, and animations
- **No Build Step**: Runs directly in browser, no bundlers needed

### Game Architecture
```
Game Loop (60 FPS via requestAnimationFrame)
├── Input Handler (keyboard state tracking)
├── Update Phase
│   ├── Player physics & shooting
│   ├── Enemy AI & formation movement
│   ├── Bullet collision detection
│   └── Explosion particles
└── Render Phase
    ├── Background (star field)
    ├── Game objects (enemies, player, bullets)
    └── Post-processing (CRT effects via CSS)
```

### Key Technical Features
- **Delta-time based physics**: Consistent speed across frame rates
- **Rectangular collision detection**: Efficient hit testing
- **Object pooling**: Reusable bullet/explosion arrays
- **Local Storage**: Persistent high score
- **Responsive CRT overlay**: CSS-based scanline effect

---

## 📁 Project Structure

```
galaga-clone/
├── index.html      # Complete game (HTML + CSS + JS)
├── README.md       # This file
└── .gitignore      # Git ignore file
```

---

## 🔧 Browser Support

| Browser | Version | Status |
|---------|---------|--------|
| Chrome | 80+ | ✅ Tested |
| Firefox | 75+ | ✅ Tested |
| Safari | 13+ | ✅ Tested |
| Edge | 80+ | ✅ Tested |

---

## 📜 License

MIT License - Feel free to use, modify, and distribute.

---

## 🙏 Credits

- **Original Game**: Namco's Galaga (1981)
- **Clone Author**: Mark
- **Inspiration**: Classic arcade era of the early 1980s

---

<div align="center">

**Made with ❤️ and pure HTML5 Canvas**

*Insert Coin to Continue...*

</div>
