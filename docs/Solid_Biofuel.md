Create Solid BioFuel from Leaves and Wood
```mermaid
graph TD
    A[Storage] -->|Wood| B[Constructor]
    C[Storage] -->|Leaves| D[Constructor]
    B -->|Biomass| E[Constructor]
    D -->|Biomass| E[Merger]
    E -->|Biomass| F[Constructor]
    F -->|Solid Biofuel| G[Storage]
```