# Pathway Propagation (Biological Inspiration)

## How It Works
Inspired by biological neurons and action potentials:

- Nodes are connected in a **directed graph** (can be cyclic for recurrent thought)
- When a node "fires" (produces output), it sends a signal to all connected nodes
- The signal carries:
  - The output content
  - An **activation value** (0.0 – 1.0)
  - Timestamp
- Receiving nodes decide whether to fire based on:
  - Incoming activation strength
  - Their own threshold
  - Current emotional/priority state (from Amygdala)

## Benefits
- Creates organic "thought chains"
- Allows emergent reasoning patterns
- Mimics how humans think in cascades rather than single forward passes
- Enables **multi-hop reasoning** naturally

## Implementation Notes
Use a graph database (Neo4j, Memgraph) or in-memory graph (NetworkX + custom propagation engine).