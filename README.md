# RoamKit

Greenfield eSIM platform — **WSL-first** development workspace.

## Repos (ciljna struktura)

`
~/projects/roamkit-net/
├── roamkit-infra/   ✅ Faza -1a (bootstrap, compose, nginx, CI)
├── roamkit-docs/    ✅ Faza -1b (ADR, standardi)
├── roamkit-api/     ⏳ Faza 0
└── roamkit-web/     ⏳ Faza 0
`

## Plan

Glavni razvojni plan: [docs/ROAMKIT_DEV_PLAN.md](docs/ROAMKIT_DEV_PLAN.md) → **`.cursor/plans/roamkit.plan.md`**

## Pravila

- Agent workflow: [`AGENTS.md`](./AGENTS.md) (isti fajl u svakom repou)
- Sve naredbe (git, docker, npm, gh) **samo iz WSL-a** — nikad iz PowerShella
- Kod u ~/projects/roamkit-net/, ne u /mnt/c/
- Telecom26 (Windows) = poslovna arhiva — odvojeno od ovog workspacea

## Cursor

Otvori ovaj workspace iz WSL-a:

`ash
cd ~/projects/roamkit-net
cursor .
`

## Sljedeći korak

**Faza 0** — vidi [.cursor/plans/roamkit.plan.md](.cursor/plans/roamkit.plan.md): `roamkit-api` + `roamkit-web` skeleton → GHCR → prvi staging deploy.
