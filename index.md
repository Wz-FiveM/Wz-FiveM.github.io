
## Documentation RageUI

La documentation n'est pas terminée elle sera souvent à jour hésiter pas à Star le repo pour être au courant des mises à jour

# Exemple de fxmanifest.lua

```lua
fx_version 'adamant'
game 'gta5'

author 'Shazuub'

client_scripts {
 "RageUI/RMenu.lua",
 "RageUI/menu/RageUI.lua",
 "RageUI/menu/Menu.lua",
 "RageUI/menu/MenuController.lua",
 "RageUI/components/*.lua",
 "RageUI/menu/elements/*.lua",
 "RageUI/menu/items/*.lua",
 "RageUI/menu/panels/*.lua",
 "RageUI/menu/windows/*.lua",
}
```

# Menu

```lua
local Menu = RageUI.CreateMenu('Titre', 'Sous Titre')
```

# SubMenu

```lua
local SubMenu = RageUI.CreateSubMenu(Menu, 'Titre', 'Sous Titre')
```
