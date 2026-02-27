# Void Patrol

A top-down shooter with mouse-aimed combat, dash mechanics, and wave-based progression. Single HTML file, zero dependencies.

The sequel (or spiritual successor) to [Void Survivor](https://github.com/sisiphamus/void-survivor-game), Void Patrol adds mechanical depth with a dash system, combo tracking, pickup magnets, and boss fights every 5 waves.

## Gameplay

- **WASD movement** with **mouse-aimed crosshair shooting**
- **Dash mechanic** with cooldown (180 frames) for burst repositioning
- **Invincibility frames** (60 frames) after taking damage, so getting hit once doesn't chain into instant death
- **Combo window** (90 frames) rewarding aggressive play with streak bonuses
- **Pickup magnet system** with configurable range for collecting drops
- **Boss fights** every 5 waves with tougher enemies
- **Upgrade shop** between waves (indicated by the "buy" sound effect in the audio engine)

## Under the Hood

Like Void Survivor, everything is self-contained:

- **All audio synthesized** via Web Audio API at runtime (shoot, hit, explode, pickup, buy, death, wave-start)
- **Canvas rendering** with pixel-art mode (`image-rendering: pixelated; crisp-edges`) for a retro aesthetic
- **Screen shake** with 0.88 decay factor for impact feedback
- **Responsive canvas** scaling to fill the browser window
- **Well-organized config object** (`CFG`) for easy balance tuning of speeds, HP, cooldowns, and damage values

## Tech

HTML5 Canvas, vanilla JavaScript, Web Audio API. Single file, zero dependencies.
