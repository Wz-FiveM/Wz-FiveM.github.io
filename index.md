
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
```md
| Nom      | instruction                   | Exemple              |
|----------|-------------------------------|----------------------|
| model    | Hash ou "nom"                 | GetHashKey("sultan") |
| position | Position du spawn du véhicule | vector3(0,0,0)       |
| heading  | Heading du spawn du véhicule  | 150.0                |
| cb       | Callback                      | function(vehicle)   |
```

 #### Exemple
```lua
NCS.spawnVehicle("sultan", vector3(0,0,0), 150.0, function(vehicle)
    FreezeEntityPosition(vehicle, true)
end)
```
