
## Documentation NCS Framework

La documentation sera totalement finit à la sortie du framework

# GetJob

```lua
local Job = NCS.getPlayerJob()
```

# GetPosition

```lua
local pPos = NCS.getPlayerPos()
```
# Spawn Veh
```lua
NCS.spawnVehicle(model, position, heading, cb, inNetwork)
```
| Nom      | instruction                   |
|----------|-------------------------------|
| model    | Hash ou "nom"                 |
| position | Position du spawn du véhicule |
| heading  | Heading du spawn du véhicule  |
| cb       | Callback                      |
| inNetwork| Si le véhicule doit être dans le réseau |
