# Build State

| Field | Value |
| --- | --- |
| Project | NEON HORIZON 2088 — Cyberpunk 3D Pinball Studio (`neon-horizon-2088`) |
| Started | 2026-11-01 03:47:45 UTC |
| Packaged | 2026-11-01 04:34:10 UTC |
| Duration | **46m 24s** (2,784 seconds) |
| Harness | OpenCode 2.2.5 |
| Model | DeepSeek V4.1 Flash (`opencode-go/deepseek-v4.1-flash`) |
| Session | `ses_e6ac7942effe0GS7Yi86hbJntl` |
| Repository | <https://github.com/somphol/neon-horizon-2088> |
| Live demo | <https://somphol.github.io/neon-horizon-2088/> |

## Token usage

| Metric | Tokens |
| --- | ---: |
| Input | 463,762 |
| Output | 118,984 |
| Reasoning | 102,748 |
| **Total (input + output + reasoning)** | **685,494** |
| Cache read | 44,503,936 |
| Cache write | 1,218 |
| Total including cache | 45,190,648 |

> Snapshot taken from the OpenCode session record when the project was packaged at 2026-11-01 04:34:10 UTC. The final commit, push, Pages verification and closing response happen outside this snapshot, so the live session totals will be marginally higher. Total cost reported by the session: **$0.00**.

## What was built

- A complete 3D cyberpunk pinball game in three modular files:
  - `index.html` — 13,619 bytes, 259 lines
  - `style.css` — 43,864 bytes, 1926 lines
  - `script.js` — 124,776 bytes, 3583 lines
- An inclined 6.6° glass-topped cabinet with a matte-black chassis, chrome rails, legs, backglass marquee, neon underglow, city skyline and grid floor.
- Procedural playfield art: circuit traces, node rings, lane arrows, warning bands and a sector watermark, drawn to a 1024 × 2048 canvas.
- Three Quantum Plasma Cores (cyan, magenta, violet) with point-light flashes, emissive pulses, scale pops, spark bursts and outward physics kicks.
- Four Cyber Security drop targets: scoring hits, bank clear bonus, multiplier increase up to ×8 and timed re-arm.
- Two translucent neon-purple Hyper-Loops with trigger sensors, Catmull-Rom rail rides and tangent release toward the flippers.
- Railgun plunger with keyboard hold/release and touch hold/drag; spring compression animation, charge meter and rising charge oscillator.
- Dual kinematic flippers with pivots, angular velocity transfer, neon edges and key/touch mapping.
- Chrome fusion ball with a generated reflection environment, dynamic glow, point light and comet trail.
- Slingshots, pegs, outlanes, drain detection, stuck-ball rescue, speed clamp and 120 Hz fixed-step simulation.
- 100% synthesised Web Audio: ambient hum, laser/plasma bumper voices, flipper thunks, target chirps, loop whooshes, drain, multiplier arpeggio, extra ball and game-over chord.
- localStorage leaderboard, callsign and mute persistence; top-five HUD and 30-entry archive.
- `neon_horizon_scores.json` export and validated merge import, with HTML stripping and de-duplication.
- Glassmorphic HUD with score, multiplier, balls, best, combo, target/loop/bumper telemetry and archive controls.
- Start hero, operator manual, new-game confirmation, game-over summary and toast system.
- Responsive desktop/tablet/mobile layouts; large touch flip pads, hold-drag launch pad, slide-in score drawer and resize-safe canvas/camera.
- Built-in `?selftest=1` surface with **16/16** checks.

## Verification

- **16/16** self-tests pass: formatting, sanitisation, Three.js/Cannon.js presence, table tilt, 3 cores, 4 targets, 2 loops, 2 flippers, ball collider, physics world, storage, serialisation, audio API and export filename.
- Headless Chrome end-to-end runs verified:
  - full-charge railgun launch through the curved lane guide,
  - Hyper-Loop capture, rail ride and flipper-side release,
  - plasma core hit, light flash, sparks and outward kick,
  - drop-target hit, bank clear, multiplier increase and re-arm,
  - left/right flipper motion and ball momentum transfer,
  - slingshot hits,
  - drain → ball countdown → respawn,
  - three-ball game over, auto-archive, final summary and archive rank,
  - `neon_horizon_scores.json` export and merge import,
  - callsign, audio mute and leaderboard persistence,
  - mobile touch launch and touch flippers,
  - viewport resize 1600×1000 → 768×1024 → 390×844 → 320×568,
  - **0** uncaught exceptions and **0** console errors in the final run.
- Screenshots: `screenshot.png` (1600×1000), `screenshot-mobile.png` (390×844 @2×), `screenshot-start.png` (1600×1000).

## Files

| File | Size |
| --- | ---: |
| `index.html` | 13,619 bytes |
| `style.css` | 43,864 bytes |
| `script.js` | 124,776 bytes |
| `README.md` | 16,165 bytes |
| `screenshot.png` | 838,590 bytes |
| `screenshot-mobile.png` | 780,163 bytes |
| `screenshot-start.png` | 564,346 bytes |

## Credits

Built with [OpenCode](https://opencode.ai) 2.2.5 and **DeepSeek V4.1 Flash** (`opencode-go/deepseek-v4.1-flash`) in a single agent session. The game code, cabinet and playfield geometry, procedural textures, physics tuning, HUD, audio synthesis, score archive and verification harness were generated for this project.

Runtime libraries: [Three.js](https://threejs.org/) r128 (MIT) and [Cannon.js](https://schteppe.github.io/cannon.js/) 0.6.2 (MIT). Typefaces: **Orbitron** and **Rajdhani** from Google Fonts (SIL OFL 1.1). No image, texture, audio or 3D model assets were used. See [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).
