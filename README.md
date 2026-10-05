# interactor-aria-patrol-solver

An Elixir application that plans patrol routes through scattered waypoints with a hierarchical task planner and writes the trajectory as JSON.

## What it is for

It places waypoints on a grid maze or a sphere, orders their visits to shorten the route, and walks the route over a navigation mesh with the planner's locomotion domain. Domains and plans import from and export to HDDL. The trajectory JSON feeds a 3D viewer, and `docs/` covers that step. `mix help patrol_solve` lists the task's options.

## Build and run

```sh
mix deps.get
mix patrol_solve
```

## Licence

MIT; see `LICENSE`.
