# SIGNAL-AV

**ASL intent bridge for autonomous-vehicle interfaces.**

SIGNAL-AV explores how signed or accessible human communication can be normalized into **safe, auditable context** for autonomous-driving systems.

> **Status: architecture/prototype track.** This repository does not control a vehicle and must not be represented as an autonomous-driving safety certification.

## Reference flow

```text
ASL / gesture / accessible input
        |
        v
local perception + confidence
        |
        v
normalized intent
        |
        v
vehicle-context adapter
        |
        v
external safety / authority controller
```

The accessibility layer may express intent such as “stop,” “help,” or “I need assistance,” but it does not itself receive steering, braking, navigation, or emergency-dispatch authority.

## Production requirements

- provenance for sensors/models/components,
- confidence thresholds and human/fallback behavior,
- no raw biometric retention by default,
- simulation before any physical integration,
- explicit vehicle-controller authorization,
- reproducible latency/accuracy/safety benchmarks.

See [PRODUCTION_READINESS.md](PRODUCTION_READINESS.md).

---

**Unmute1AI**  
Signal, not assumption.
