# Sunset Circuit

An original browser kart racer inspired by Mario Kart 8. Race eleven computer drivers for three laps across three original circuits.

[Play online](https://intrepion.github.io/kata-inspired-by-mario-kart-8-codex-dot/) · [Kata Arcade](https://intrepion.github.io/)

## Controls

- **Up / W** accelerate; **Down / S** brake
- **Left / Right** or **A / D** steer
- Hold **Space** or **Shift** while steering to drift; release after sparks appear for a boost
- **X** uses the active item; **C** swaps active and reserve items; **P** pauses; **R** returns the kart to the track
- Touch controls appear on touch devices. Hold GO to accelerate, tap ITEM to use the active item, and tap SWAP to select the other slot. Use the Reset button to return to the track.

Time acceleration during the countdown for a rocket start. Collect up to ten coins for extra top speed. Item boxes fill up to two slots with a boost, a peel to drop behind, a straight-flying DART, or a homing SEEKER that tracks a nearby rival ahead. Swap slots freely; using an item automatically selects the other occupied slot. Select Sunset Circuit, Copper Canyon, or Moonlight Harbor before starting. Cones, moving boulders, and sweepers spin you out and cost coins on contact. Grass slows the kart down; the kart is returned to the course after spending too long off-road. Drifts charge blue, orange, then pink boosts.

Four original synthesized themes—one for the menu and one for each course—are off by default. Use **Music off/on** and the volume slider below the game to control it. Music changes between the menu and the selected course, with a brief fade between themes.

## Run locally

Serve this directory with `python3 -m http.server` and visit `http://localhost:8000/`. Three.js is vendored in `vendor/`, so the game needs no network connection after loading.

## Scope

This is a small, original arcade interpretation, not a reproduction of Mario Kart 8. It has three 3D circuits, one player, eleven computer racers, four item types, and no multiplayer, gliding, anti-gravity, tricks, vehicle selection, or Nintendo assets. Item targeting and opponents are simplified: DARTs travel straight and SEEKERs home toward a nearby rival ahead; AI attacks are abstract rather than simulated projectiles. Driving and drift physics are original approximations, not Mario Kart 8 physics.

## License

MIT; see [LICENSE](LICENSE). The game is unaffiliated with Nintendo.

## Development

Run `node tests/smoke.cjs` for a headless simulation of steering through a complete three-lap race, drift and item activation. It does not replace browser playtesting. Three.js 0.180.0 is included under its MIT license in `vendor/THREE-LICENSE.txt`.

## Arcade metadata

See [docs/arcade-metadata.md](docs/arcade-metadata.md) for the game-owned manifest and screenshot provenance.
