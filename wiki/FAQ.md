# FAQ

## My signal stays red. Why?

Right-click it: it tells you the reason. The most common ones:

| Reason | Meaning | What to do |
|---|---|---|
| `BLOCK_OCCUPIED` | A cart, mob or player is in the block ahead. | Clear the block; check for a forgotten cart. |
| `AWAITING_TRAIN` | Nothing is approaching. Signals show STOP until a train asks for the block. | Nothing; it clears for an approaching train. |
| `NO_ROUTE` | The train's destination cannot be reached from here. | Check the track and switch motors on the way. |
| `UNKNOWN_CHUNK` | Part of the block lies in an unloaded chunk. | Load the area; unknown is always stop. |
| `NO_SAFE_EXIT` | A chain signal sees no free exit behind the next signal. | Clear the block behind the next signal. |
| `RECOVERY_REQUIRED` | After a restart the train is not identified yet. | Wait a moment; trains are recognised again on their own. |

## A cart stops between two stations.

Vanilla minecarts lose speed. Every signal that clears in front of a cart launches it again, and departing trains
are launched too, but on long open stretches you need powered rails, transport rails or a cart engine.

## The other mod's rails / carts do not work with signals.

By default the network only trusts vanilla rails and minecarts and those of Signals Reforged. Rails of other mods are
unknown (signals stay at STOP), carts of other mods count as obstacles. A server operator can add a tested mod to
`trustedRailNamespaces` or `trustedCartNamespaces`; see [Configuration](Configuration).

## I cannot use the signal box / throw a switch / create cargo orders.

On a server, actions need a role (operators can always act). An owner or operator gives roles in the rights window
(button "Rights..." in the diagnostics view of a console) or with `/signals role`. See
[Commands and Permissions](Commands-and-Permissions). Viewing is free.

## Does the mod load chunks?

No, unless an operator turns it on (`chunkLoading.enabled`). Then the Chunkloader Upgrade keeps chunks around a cart
with an order loaded, limited per player and with an idle timeout.

## Can I copy a layout with a structure block or a world editor?

Yes. Copied station markers become new stations with the same names, and repeaters and rail links point at the copied
blocks. Rotated copies work (structure block or `/place template`); mirrored copies do not. A station moved this way
counts as a new station: update lines and tickets that used the old one.

## Is my world safe when I update?

Back up your world before every update, especially during the beta. The save data carries a schema version; an
unknown newer version is not overwritten.

## Is there a Fabric version?

Not yet. It is planned after the NeoForge version is complete.
