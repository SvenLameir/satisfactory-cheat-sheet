# Starter Layouts
## Concrete Starter
120 Limestone in  
45 Concrete out
```mermaid
graph TD
    A[Miner] -->|120 Limestone/min| B1[Splitter]
    B1 -->|45 Limestone/min| C1[Constructor 100%]
    B1 -->|45 Limestone/min| C2[Constructor 100%]
    B1 -->|30 Limestone/min| C3[Constructor 66.666%]
    C1 -->|15 Concrete/min| D[Merger]
    C2 -->|15 Concrete/min| D
    C3 -->|10 Concrete/min| D
    D -->|40 Concrete/min| E[Storage]
```

## Iron Starter
120 Iron Ore in  
60 Iron Plate, 20 Iron Rod, 40 Screw out
```mermaid
graph TD
    A[Miner] -->|120 Iron Ore/min| B(4x Smelter)
    B -->|90 Iron Ingot/min| C(3x Constructor)
    B -->|30 Iron Ingot/min| D(2x Constructor)
    C -->|60 Iron Plate/min| E[Storage]
    D -->|20 Iron Rod/min| F[Storage]
    D -->|10 Iron Rod/min| G[1x Constructor]
    G -->|40 Screw/min| H[Storage]
```

## Copper Starter
120 Copper Ore in  
60 Wire, 30 Cable, 30 Copper Sheet out
```mermaid
graph TD
    A[Miner Mk.3] -->|120 Copper Ore/min| B[4x Smelters]
    B -->|60 Copper Ingots/min| C[4x Constructors]
    C -->|60 Wire/min| D[Storage]
    C -->|30 Wire/min| E[1x Constructor]
    E -->|30 Cable/min| F[Storage]
    B -->|60 Copper Ingots/min| G[3x Constructors]
    G -->|30 Copper Sheets/min| H[Storage]
```

## Advanced Iron
Requires underclocking but Will get the job done early game  
105 Iron Ore in  
3 Reinforced Iron Plate, 2 Rotor, 2 Smart Plating out
```mermaid
graph TD
    A[Miner] -->|105 Iron Ore/min| B[3.5 Smelter]
    B -->|45 Iron Ingot/min| C[1.5 Constructor]
    B -->|60 Iron Ingot/min| D[4 Constructor]
    C -->|30 Iron Plate/min| E[1 Assembler]
    E -->|3 Reinforced Iron Plate/min| F[Storage]
    D -->|20 Iron Rod/min| E
    D -->|40 Iron Rod/min| G[4 Constructor]
    G -->|100 Screw/min| H[1 Assembler]
    G -->|60 Screw/min| E
    H -->|2 Rotor/min| I[1 Assembler]
    E -->|2 Reinforced Iron Plate/min| I
    I -->|2 Smart Plating/min| J[Storage]
    H -->|2 Rotor/min| K[Storage]
```

## Modular Frame
120 Iron Ore in  
5 Modular Frame/min out
```mermaid
graph TD
    A[Mine] -->|120 Iron Ore/min| B[4 Smelters Iron Ingot]
    B -->|67.5 Iron Ingot/min| C[2.25 Constructor]
    B -->|52.5 Iron Ingot/min| D[3.5 Constructor]
    C -->|45 Iron Plate/min| E[1.5 Assembler]
    D -->|30 Iron Rod/min| E
    D -->|22.5 Iron Rod/min| F[2.25 Constructors Screw]
    F -->|90 Screw/min| E
    E -->|7.5 Reinforced Iron Plate/min| G[2.5 Assembler]
    G -->|5 Modular Frame/min| H[Storage]
```