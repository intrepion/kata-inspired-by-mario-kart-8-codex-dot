# Sunset Circuit

An original browser kart racer inspired by Mario Kart 8. Race eleven computer drivers for three laps on a sunny circuit.

[Play online](https://intrepion.github.io/kata-inspired-by-mario-kart-8-codex-dot/) · [Kata Arcade](https://intrepion.github.io/)

## Controls

- **Up / W** accelerate; **Down / S** brake
- **Left / Right** or **A / D** steer
- Hold **Space** or **Shift** while steering to drift; release after sparks appear for a boost
- **X** uses the held item; **P** pauses
- Touch controls appear on touch devices. Hold GO to accelerate.

Time acceleration during the countdown for a rocket start. Collect up to ten coins for extra top speed. Item boxes grant a boost, a peel to drop behind, or a bolt that hits a nearby rival ahead. Grass slows the kart down. Drifts charge blue, orange, then pink boosts.

## Run locally

Serve this directory with `python3 -m http.server` and visit `http://localhost:8000/`. Three.js is vendored in `vendor/`, so the game needs no network connection after loading.

## Scope

This is a small, original arcade interpretation, not a reproduction of Mario Kart 8. It has one 3D circuit, one player, eleven computer racers, three item types, and no multiplayer, gliding, anti-gravity, tricks, vehicle selection, or Nintendo assets. Item targeting and opponents are simplified: bolts affect a nearby racer ahead instantly, and AI attacks are abstract rather than simulated projectiles. Driving and drift physics are original approximations, not Mario Kart 8 physics.

## License

MIT; see [LICENSE](LICENSE). The game is unaffiliated with Nintendo.

## Development

Run `node tests/smoke.cjs` for a headless simulation of steering through a complete three-lap race, drift and item activation. It does not replace browser playtesting. Three.js 0.180.0 is included under its MIT license in `vendor/THREE-LICENSE.txt`.
