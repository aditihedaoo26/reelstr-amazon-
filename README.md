# Reelstr

Open-source serial video on Nostr, with per-episode sats and signed revenue splits.

## Project Structure

| Directory | Description |
| --- | --- |
| `apps/` | Web application and mobile app shells (Capacitor / Android / iOS) |
| `packages/` | Core packages: protocol, Nostr, Blossom, media, wallet, UI components |
| `services/` | Microservices: relay, crew relay, media, indexer, key server, split, agent |
| `demo/` | Demo stack and seed scripts |
| `e2e/` | Headless browser end-to-end tests |
| `interop/` | Interoperability readers and tools |
| `infra/` | Infrastructure, container setups, and deployment configs |
| `docs/` | Specifications, NIP documentation, and architecture notes |

## Quick Start

### Prerequisites
- [Bun](https://bun.sh)
- Go
- ffmpeg
- Chrome

### Installation & Run

```sh
bun install
(cd infra/blossom && npm install && npm rebuild better-sqlite3)
bun run demo
```

## Everyday Commands

```sh
bun run check         # lint, types and unit tests
bun run lint          # biome check
bun run fix           # biome check with auto-fixes
bun run test:e2e      # headless browser tests
```

See [CONTRIBUTING.md](CONTRIBUTING.md) for full development conventions.

## License

[MIT](LICENSE)
