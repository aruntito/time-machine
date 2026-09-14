# TIME-MACHINE Architecture

TIME-MACHINE models historical state as a function of observations over time.

## Flow

```text
OBSERVATIONS
   │
   ├── EVENTS
   ├── SNAPSHOTS
   └── PROVENANCE
        │
        ▼
 TEMPORAL NORMALIZATION
        │
        ▼
   STATE HISTORY
        │
        ▼
 POINT-IN-TIME RECONSTRUCTION
        │
        ▼
 HISTORICAL STATE + UNCERTAINTY
```

## Design principles

1. History must be reproducible from retained evidence.
2. Event time and observation time remain distinct.
3. Missing evidence is represented rather than silently inferred.
4. Reconstruction should be deterministic for the same evidence set.
5. Every reconstructed state should retain provenance.

## Boundaries

TIME-MACHINE reconstructs historical state; it does not decide causality. TRACE handles causal investigation, while BLACKBOX handles incident reconstruction.