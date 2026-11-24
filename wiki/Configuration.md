# Configuration

## Server: `config/signalsreforged-local.toml`

| Option | Default | Meaning |
|---|---|---|
| `serverSafety.allowCrossDimTeleportRail` | `false` | Teleport rails may move carts, passengers and cargo between dimensions. |
| `train.cartEngineBlacklist` | TNT and command block minecarts | Minecart types that may not get a cart engine. |
| `train.maxConsistLength` | `8` | Maximum number of carts in one coupled train (1 to 32). |
| `chunkLoading.enabled` | `false` | Chunkloader upgrades may load chunks around carts with a valid order. |
| `chunkLoading.maxActiveTrainChunkTicketsPerOwner` | `4` | Carts per player that may load chunks at the same time. |
| `chunkLoading.radius` | `1` | Chunks around a loading cart: 0 = its chunk, 1 = 3 x 3, 2 = 5 x 5. |
| `chunkLoading.idleTtlTicks` | `6000` | A cart that has not moved for this many ticks stops loading chunks. |
| `compatibility.trustedRailNamespaces` | `minecraft`, `signalsreforged` | Mods whose rails count like vanilla rails. Add a mod only after testing it. |
| `compatibility.trustedCartNamespaces` | `minecraft`, `signalsreforged` | Mods whose minecarts the interlocking may hold, launch and route. |
| `cargo.cancelledVisibleSeconds` | `60` | How long cancelled and failed orders stay in the lists. |
| `cargo.deliveredVisibleSeconds` | `600` | How long delivered orders stay in the lists. |

## Client: `config/signalsreforged-client.toml`

| Option | Default | Meaning |
|---|---|---|
| `fxQuality` | `HIGH` | Particles: HIGH = all, LOW = only state markers, OFF = none. Signal states stay visible in every mode. |
| `reducedMotion` | `false` | Arms, flaps, levers and switch rods jump to their end position. |
| `colorblindAssist` | `false` | Colour-blind friendly lamp colours plus a letter on every lit lamp. |
| `glowIntensity` | `1.0` | Brightness of lamp glows (0 to 1). |

The mod also ships a "3D rails" resource pack that is switched on once at the first start; switch it in
Options > Resource Packs. The emergency call key (default **N**) is in the controls settings.
