# Void Patrol

1,816 lines of JavaScript. One HTML file. No build step, no dependencies, no assets on disk. You open it in a browser and you're dodging bullets.

This is a top-down shooter where you aim with the mouse, move with WASD, and dash through danger on a 3-second cooldown. Every sound in the game -- the 800-to-200Hz frequency sweep when you shoot, the sawtooth growl when a boss spawns, the ascending C-E-G chime when you buy an upgrade -- is synthesized at runtime from raw oscillators and noise buffers. Nothing is prerecorded. The Web Audio API is doing all of it.

Between waves you spend credits at the upgrade shop: hull plating, thrusters, fire rate, power, bullet velocity, multi-shot, shields, and a pickup magnet. Costs scale exponentially so you're always making tradeoffs. Every 5 waves a boss shows up -- 40 HP, phase shift at half health, fires back at you every 40 frames. The screen shakes with a 0.88 decay factor on every impact, which sounds like a small number until everything is exploding at once.

Enemy variety keeps it interesting. Grunts chase you down. Dashers zigzag in fast. Tanks absorb punishment and shoot back. Snipers kite at range. Bombers rush you. And the boss does all of it.

Sequel to [Void Survivor](https://github.com/sisiphamus/void-survivor-game), which proved the concept. This one has the depth.

`index.html` -- that's the whole repo.
