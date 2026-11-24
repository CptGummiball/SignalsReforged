# Example layouts

Small, working layouts for the main features. Each one comes with screenshots, a step-by-step "try it", its material
list and a structure file. The structures ship inside the mod, so you can place any of them in a creative world:

```
/place template signalsreforged:wiki/<name> ~ ~-1 ~
```

| Layout | Shows | Name |
|---|---|---|
| [Block signals on a line](Layout-Block-Signals) | ![](images/block_signals_overview.jpg) | `block_signals` |
| [Junction with chain and path signals](Layout-Junction) | ![](images/junction_overview.jpg) | `junction` |
| [Passing loop with detour](Layout-Passing-Loop) | ![](images/passing_loop_overview.jpg) | `passing_loop` |
| [Rail crossing protected by signals](Layout-Rail-Crossing) | ![](images/rail_crossing_overview.jpg) | `rail_crossing` |
| [Station with two platforms](Layout-Station-Platforms) | ![](images/station_platforms_overview.jpg) | `station_platforms` |
| [Cargo line with docks, buffer and cart hopper](Layout-Cargo-Line) | ![](images/cargo_line_overview.jpg) | `cargo_line` |
| [Signal box and control devices](Layout-Control-Room) | ![](images/control_room_overview.jpg) | `control_room` |
| [Transport rails, limiter rails and a rail link](Layout-Special-Rails) | ![](images/special_rails_overview.jpg) | `special_rails` |

All pictures come from a real game: the layouts are built and run by the development client
(`./gradlew runClient -Psignals.wiki=true`), which also exports the structures and material lists
(`python tools/wiki_layouts.py` then copies the pictures and fills the tables).
