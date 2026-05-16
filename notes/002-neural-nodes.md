# Neural Nodes

## Core Concept
Each **Neural Node** is a self-contained mini-LLM agent with:

- **Specialized System Prompt** (defines its role and expertise)
- **Local Context Window** (short-term memory)
- **Activation State** (on / off / firing)
- **Connections** to other nodes (weighted synapses)

## Node Lifecycle
1. Query arrives → Relevant nodes are activated
2. Node processes input with its mini-LLM
3. Node outputs a structured thought / memory fragment
4. State propagates to connected nodes
5. Results are aggregated and passed to main model

## Mini-LLM Ideas
- Use small open models (Phi-3, Gemma-2B, TinyLlama, etc.)
- Or distilled versions of larger models fine-tuned per region
- Future: Mixture-of-Experts at node level