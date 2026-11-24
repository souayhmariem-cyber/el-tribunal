# El Tribunal

El Tribunal is an immersive, gamified cybersecurity education platform. Players act as cyber-detectives, investigate incidents, examine evidence, build timelines and hypotheses, and submit incident reports.

## Product direction

- **Experience:** detective investigations combined with an interactive 3D network city.
- **Visual identity:** vintage detective noir meets futuristic cyberpunk.
- **Cases:** five independent investigations; each case can be played without completing another.
- **Architecture:** one reusable investigation engine driven by case configuration and server-owned state.

## Technology stack

| Layer | Technology |
|---|---|
| Frontend | React.js |
| Backend | Node.js, Express.js |
| Database | MySQL |
| 3D experience | Three.js, React Three Fiber |

## Repository layout

- `client/` — browser application and user interface.
- `server/` — API, application rules, persistence, and server-side evaluation.
- `shared/` — contracts and constants shared across client and server.
- `docs/` — architecture and engineering documentation.
- `case-materials/` — approved, non-sensitive case specifications and player-safe content.

## Security principles

1. The server is authoritative for investigation state, evidence unlocks, scoring, and evaluation.
2. Creator-only truth, answer keys, hidden motives, and grading logic must never be shipped to the browser.
3. Do not trust client-submitted scores, conclusions, timestamps, or evidence-unlock claims.
4. Keep secrets in environment variables; never commit credentials or production data.
5. Treat the original creator case files as source material. Do not copy them into the frontend or public assets.

## Development status

The repository is being bootstrapped. Application features and dependencies will be introduced in reviewed, focused changes. See [CONTRIBUTING.md](CONTRIBUTING.md) and [docs/architecture/README.md](docs/architecture/README.md).

## Getting started

The project scaffold is not yet wired to runnable client or server applications. Setup instructions will be added when the first application packages are introduced.
