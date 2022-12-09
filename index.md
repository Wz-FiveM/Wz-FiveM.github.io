## Documentation RedFramework V2.0

# Import Libs Client and Server Side

```lua
local RedFramework = exports["redFrameworkV2"]
```

# Server Side

# GetPlayer
```lua
local player = RedFramework.getPlayer(playerId)
```

```lua
local job = player.getJob()
```
```lua
local inventory = player.getInventory()
```
```lua
local accounts = player.getAccounts()
```
```lua
local group = player.getGroup()
```


Exemple
```lua
RegisterCommand('getPlayerInventory', function(source, args)  
    local player = RedFramework.getPlayer(source)
    local inventory = player.getInventory()
    print(json.encode(inventory.data))
end)
```

| Argument           | Type   |
|--------------------|--------|
| playerID or source | number |
