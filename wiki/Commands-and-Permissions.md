# Commands and Permissions

## Roles

Every player can ride to **public** stations. Everything else needs a role on the network (or on a single station or
depot). Server operators (permission level 2) always act as admin. Each role includes the rights of the roles above it
in this table:

| Role | May |
|---|---|
| Viewer | see the network in consoles |
| Operator | request routes, manage cargo orders, trigger an emergency stop |
| Dispatcher | also block signals, throw switches, edit lines and timetables, rename stations |
| Owner | also configure devices and districts, release emergency stops, change roles |

Roles are changed in the **rights window** (button "Rights..." in the diagnostics view of the signal box, the network
controller or the tablet) or with `/signals rights` and `/signals role`. The last owner of a network cannot be
removed. Stations can be set to private in the station screen; private stations need a role to be a destination.

## Commands

| Command | Who | What |
|---|---|---|
| `/signals status` | everyone | state of the network in this dimension |
| `/signals scan-local [radius]` | everyone | network facts around you |
| `/signals rights` | everyone | opens the rights window |
| `/signals role <player> <role> [station <name> \| depot <name>]` | owner | gives a role on the network, a station or a depot |
| `/signals calls` · `/signals calls release <train>` | dispatcher | open emergency calls from passengers |
| `/signals emergency on` · `off` | operator / owner | network-wide emergency stop and its release |
| `/signals rescan` | operator (server) | rescans the track network |
| `/signals validate` | operator (server) | checks the network and lists problems |
| `/signals repair` | operator (server) | repairs inconsistent saved data |
| `/signals chunkloads` | operator (server) | carts that currently load chunks |
| `/signals diagnostics export [full]` | operator (server) | writes a diagnostics report (without player names unless `full`) |
