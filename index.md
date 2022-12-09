## Documentation RedFramework V2.0

# Import Libs Client and Server Side

```lua
local RedFW = exports["redFrameworkV2"]
```

# Server Side

```lua
local player = RedFW.getPlayer(playerId)
```

```lua
player.getJob()
```
```lua
player.getInventory()
```
```lua
player.getAccounts()
```
```lua
player.getGroup()
```


Exemple
```lua
RegisterCommand('getPlayerInventory', function(source, args)  
    local player = RedFW.getPlayer(source)
    local inventory = player.getInventory()
    print(json.encode(inventory.data))
end)
```
# Server Functions
```lua
---@param message: string
---@param type: string
RedFW.makeTrace(message, type)
```
```lua
---@param serverId: number
RedFW.getIdentifier(serverId)
```
```lua
---@return: table
RedFW.getAllPlayers()
```
```lua
---@param name: string
---@param callback: function
---@param forStaff: boolean
RedFW.registerCommand(name, callback, forStaff)
```

# Client Side

```lua
---@return number
RedFW.getCash()
```
```lua
---@return number
RedFW.getBank()
```
```lua
---@return table
RedFW.getJob()
```
```lua
---@return table
RedFW.getInventory()
```
```lua
---@return table
RedFW.getAccounts()
```
```lua
---@return table
RedFW.getGroup()
```
```lua
---@return number
RedFW.getBlackMoney()
```
```lua
---@return table
RedFW.getSkin()
```
```lua
---@param skinTable table
---@return void
RedFW.loadSkin(skinTable)
```
```lua
RedFW.saveSkin()
```
```lua
---@param key string
---@param value number
---@return void
RedFW.changerSkinKey(key, value)
```
