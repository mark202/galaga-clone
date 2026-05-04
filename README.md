# Galaga Clone

A complete, fully playable Galaga clone built with pure HTML5 Canvas and vanilla JavaScript.

![Game Screenshot](https://via.placeholder.com/480x640/000/0f0?text=GALAGA+CLONE)

## Features

### Gameplay
- **Player Ship**: Cyan spacecraft with smooth movement and rapid-fire shooting
- **Two Enemy Types**:
  - **Bee (Yellow)**: Fast, erratically swooping attackers - 100 points
  - **Butterfly (Magenta)**: Slower, curved attack patterns, takes 2 hits - 150 points
- **Classic Galaga Formations**: Enemies spawn in iconic grid patterns and swoop down in waves
- **Enemy Shooting**: Enemies fire red bullets that the player must dodge
- **Wave/Level Progression**: Each wave adds more enemies, faster movement, and more aggressive shooting
- **3 Lives System**: Game over when all lives are lost

### Visual Effects
- **Parallax Star Field**: Animated scrolling background with 100 stars at varying depths
- **Explosion Particles**: Colorful burst animations when enemies or player are hit
- **CRT Scanline Effect**: Authentic retro arcade monitor appearance
- **Screen Curvature**: Subtle vignette effect for that classic cabinet feel
- **Screen Shake**: Impact feedback when the player is hit
- **Neon Glow UI**: Classic arcade-style neon green text and borders

### Technical Features
- **60 FPS Gameplay**: Smooth animation using `requestAnimationFrame`
- **Collision Detection**: Pixel-accurate hit detection for bullets and ships
- **Session High Score**: Tracks your best score during the session
- **Game States**: START_SCREEN, PLAYING, WAVE_CLEAR, and GAME_OVER screens

## Controls

| Key | Action |
|-----|--------|
| **Arrow Left / A** | Move ship left |
| **Arrow Right / D** | Move ship right |
| **Space** | Shoot / Start game / Restart |

## How to Play

1. Open `index.html` in any modern browser
2. Press **Space** to start the game
3. Move your ship to avoid enemy bullets
4. Shoot down the Bee and Butterfly enemies before they overwhlem you
5. Clear all waves to progress and increase your score multiplier
6. Survive as long as possible and beat your high score!

## Scoring

| Enemy Type | Points | Notes |
|------------|--------|-------|
| Bee | 100 | Fast, erratic movement |
| Butterfly | 150 | Takes 2 hits to destroy |

## Difficulty Progression

Each wave increases:
- **Enemy count**: More Bees and Butterflies spawn
- **Attack speed**: Enemies swoop faster
- **Shooting frequency**: More aggressive enemy fire
- **Movement speed**: Butterflies become more maneuverable

## Browser Compatibility

Works in all modern browsers supporting HTML5 Canvas:
- Chrome 10+
- Firefox 4+
- Safari 4+
- Edge 12+
- Opera 12+

No external dependencies required - just open `index.html`!

## File Structure

```
/tmp/galaga-clone/
├── index.html    # Complete game (single file)
└── README.md     # This documentation
```

## Architecture

The game is organized into these main components:

- **Star Field System**: Parallax scrolling background
- **Player Controller**: Movement and shooting logic
- **Enemy System**: Two enemy types with distinct attack patterns
- **Bullet System**: Player and enemy projectiles
- **Collision Detection**: Hit detection between all game entities
- **Particle System**: Explosion effects
- **CRT Effect Layer**: Post-processing for authentic retro look
- **State Machine**: Manages game flow between screens

## License

This is a fan-made tribute to Namco's classic Galaga. All game mechanics are inspired by the original 1981 arcade classic.
