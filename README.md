# TIME-MACHINE

**Historical state reconstruction for complex systems.**

> How did we get here?

TIME-MACHINE explores how to reconstruct the state of a system at a past point in time from events, snapshots, provenance, and historical observations.

## What it does

- reconstruct point-in-time state
- correlate events and snapshots
- preserve historical provenance
- replay known sequences
- represent incomplete or uncertain history

## Architecture

```text
EVENTS + SNAPSHOTS + PROVENANCE
              │
              ▼
      TEMPORAL NORMALIZATION
              │
              ▼
       STATE RECONSTRUCTION
              │
              ▼
       POINT-IN-TIME STATE
              │
              ▼
       HISTORICAL CONTEXT
```

## Ecosystem

`TIME-MACHINE → PULSE → TRACE → BLACKBOX → RECOVER → FIRSTLIGHT → WAKE`

`GRID` and `GHOST` provide infrastructure context; `EVAC` and `RELIEF-OS` extend the ecosystem into resilience research.

## Status

Early research and architecture.

- [Architecture](docs/architecture.md)
- [Roadmap](docs/roadmap.md)

## License

MIT.