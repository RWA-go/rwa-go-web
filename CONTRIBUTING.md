# Contributing to rwa-go-web

Thanks for your interest in contributing! This is the web dashboard for the [RWA-go](https://github.com/RWA-go) org.

## Sister repos

| Repo | Description |
|------|-------------|
| [rwa-call-core](https://github.com/RWA-Call/rwa-call-core) | Rust monitoring engine |
| [rwa-call-contracts](https://github.com/RWA-Call/rwa-call-contracts) | Soroban smart contracts |
| [rwa-go-web](https://github.com/RWA-go/rwa-go-web) | This repo - Next.js dashboard |

## Local setup

```bash
git clone https://github.com/RWA-go/rwa-go-web
cd rwa-go-web
npm install
cp .env.example .env.local
npm run dev
```

Open [http://localhost:3000](http://localhost:3000).

## Requirements

- Node.js 18+
- [Freighter wallet extension](https://www.freighter.app/) for wallet-gated features

## Branch naming

```
feat/<short-description>
fix/<short-description>
chore/<short-description>
```

## Commit style

Follow [Conventional Commits](https://www.conventionalcommits.org/):

```
feat(component): add X
fix(page): correct Y
chore: update deps
```

## TypeScript types

All types live in `types/index.ts` and must stay in sync with the Rust structs in `rwa-call-core`. Do not add fields here without a matching change in the core engine.

## Pull requests

- Keep PRs focused - one feature or fix per PR
- All pages must be mobile responsive and dark-mode compatible
- Run `npm run build` before opening a PR - zero lint errors required
