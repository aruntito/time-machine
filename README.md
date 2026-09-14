# TIME-MACHINE

**Historical state reconstruction for complex systems.**

> How did we get here?

TIME-MACHINE explores how to reconstruct what a system looked like at a past point in time from events, snapshots, provenance, and historical observations.

## Why it exists

Current state tells you where a system is. It does not necessarily tell you how it arrived there.

TIME-MACHINE makes historical context a first-class system capability so investigations can reason about **state at time T**, not only state now.

## What it does

- reconstruct point-in-time state
- correlate events and snapshots
- preserve historical provenance
- replay known sequences
- represent incomplete or uncertain history

## Use cases

| Use case | Question answered |
| --- | --- |
| Incident investigation | What was the system state before the incident? |
| Configuration history | When and how did this state change? |
| Deployment analysis | What was deployed at a specific time? |
| Audit / reconstruction | What can be established from historical evidence? |
| Causal analysis | What context did TRACE need to explain a change? |

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