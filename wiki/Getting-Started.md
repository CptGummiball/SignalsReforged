# Getting Started

This page builds a small line step by step. The [Example Layouts](Example-Layouts) show the same ideas as finished
builds.

## 1. Lay the track

Use normal rails and minecarts. The mod finds connected track by itself; there is nothing to register. Signals,
stations and switches only work on track that the network knows, so connect everything you want to control.

## 2. Two stations

Place a **Station Marker** directly beside a rail: that rail cell becomes a destination. Name the station by renaming
the marker in an anvil before you place it, or later in the station screen (right-click the marker). Build a second
station on the same connected track.

Markers with the same name close to each other (within 48 blocks) are **platforms of one station**; a train takes a
free platform, the one with the higher priority first.

## 3. Send a cart

* **Ticket:** right-click station markers with a Ticket to add destinations, then right-click a minecart with it.
* **Quick Ride:** board a minecart, pick a station from the list and confirm.

The cart drives to each destination in turn and stops at every station on its ticket. Carts are launched again by
every signal that clears in front of them; on long open stretches use powered rails as in vanilla.

## 4. Signals

Place a signal beside the rail **while looking in the direction trains travel**; it guards only that direction.

* **Block signal:** PROCEED only while the whole block up to the next signal is free.
* **Chain signal:** lets a train in only if it can also get out again; use it in front of junctions and crossings.
* **Path signal:** reserves the exact route through a junction for one train; other trains on routes that do not
  touch it run in parallel.

Right-click a signal to see why it shows its aspect. Sneak + right-click switches between semaphore and colour-light
style. Unknown is always stop: a block reaching into an unloaded chunk keeps its signal at STOP.

## 5. Switches

A vanilla T junction becomes a controlled switch with a **Switch Motor** placed beside the junction rail. The motor
throws the rail for routed trains and locks it while the route is reserved.

## 6. Watch and control it

The **Signal Box** (3 x 2 x 2 blocks) shows a live map of the network. Select a signal, a switch or a train to act on
it. The **Rail Network Controller** is a smaller desk for its district, the **Conductor Tablet** opens one from afar.
On a server, actions need a role; see [Commands and Permissions](Commands-and-Permissions).

## Next steps

* Departure boards, platform controllers and lines with timetables: see the layout
  [Station with two platforms](Layout-Station-Platforms).
* Cargo with loading docks: see [Cargo line](Layout-Cargo-Line).
* Coupled trains: click two carts one after the other with the **Rail Configurator**; sneak + click uncouples.
