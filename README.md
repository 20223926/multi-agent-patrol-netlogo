# Multi-Agent Patrol (EVAP & CLInG)

NetLogo simulation of multi-robot patrol on grid maps with obstacles, comparing the **EVAP** (pheromone evaporation) and **CLInG** (propagated idleness field) algorithms from Chu et al., _Swarm Approaches for the Patrolling Problem: Information Propagation vs. Pheromone Evaporation_. Agents aim to keep cell **idleness** (time since last visit) as low as possible.

## Algorithms

| Mode      | Idea                                                                                                        |
| --------- | ----------------------------------------------------------------------------------------------------------- |
| **EVAP**  | Agents deposit pheromones and prefer cells with the lowest pheromone level; pheromones evaporate over time. |
| **CLInG** | A propagated field spreads idleness across free cells; agents move toward the local maximum.                |

Metrics: **IGI** (mean idleness) and **IWI** (worst idleness).

## Requirements

- [NetLogo](https://www.netlogo.org/downloads/) 7.x

## Getting started

1. Open `model.nlogox` in NetLogo.
2. Choose a map (`Rooms`, `Spiral`, `Random`, `Blank`, or `Custom`) and an algorithm (`EVAP` or `CLInG`).
3. Run **setup**, then **go**.

Maps: `map1.png` (Rooms), `map2.png` (Spiral). You can also draw/erase obstacles in the interface or load a custom PNG.

A readable copy of the NetLogo procedures (without the UI XML) is in `patrol_evap_cling_readable.nlogox`.
