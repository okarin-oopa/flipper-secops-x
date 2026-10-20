# Architecture

Flipper SecOps X is an application suite, not a replacement firmware.

```mermaid
flowchart TD
  M[Momentum / compatible firmware] --> L[SecOps Launcher FAP]
  L --> T[Independent tools / workflows]
  T --> R[RF session logger]
  T --> A[Access inventory]
  T --> H[GPIO diagnostics]
  T --> X[Future companion protocol]
  X --> E[ESP32 / external modules]
  R --> D[Exported reports and documentation]
```

## Design decisions
- Standalone FAP first; fork only for proven API or driver requirements.
- Design for 128x64 monochrome display and five-way navigation.
- Maintain separate `docs/decisions/` records for major decisions.
- Verify licenses and firmware compatibility before integrating external apps.
