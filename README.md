### Bug Details
Ês können keine Plunderteile bei irgendeinen Hänler verkauft werden.

### Steps to Replicate
Schritt 1: k.A.
Schritt 2: k.A.
Schritt 3: k.A.

### MUI Version Info
- MUI_Core: 6.9.8
- MUI_Config: 6.9.8
- MUI_Setup: 6.9.8

### WoW Client Info
- WoW version: 10.2.5 (53262)
- Locale: deDE
- Resolution: 1920 (UI scale: 0.7)
- Using Mac: No

### Basic Character Info
- Faction: Alliance
- Class: Jäger (hunter)
- Specialization: Tierherrschaft
- Level: 64
- Race: Nachtelf

### Captured Errors (3)
- Zone: Drustvar (Gol Osigr)
- Group size: 0
- Instance type: none
- In combat: Yes
- Resting: No
- AFK: No
- Dead or ghost: No
- Timestamp: **Wed Feb 14 20:50:15 2024**

```lua
[ADDON_ACTION_BLOCKED] AddOn 'MUI_Core' tried to call the protected function 'ActionButton12:SetShown()'.
[string "../MUI_Core/Engine/Events/EventManager.lua"]:69: in function <...rface/AddOns/MUI_Core/Engine/Events/EventManager.lua:52>
[string "=[C]"]: in function `SetShown'
[string "@Interface/FrameXML/ActionBar.lua"]:195: in function `UpdateShownButtons'
[string "@Interface/FrameXML/ActionButton.lua"]:507: in function `UpdateAction'
[string "@Interface/FrameXML/ActionButton.lua"]:981: in function `OnEvent'
[string "@Interface/FrameXML/ActionButton.lua"]:207: in function <Interface/FrameXML/ActionButton.lua:204>
```
---
- Zone: Drustvar (Gol Osigr)
- Group size: 0
- Instance type: none
- In combat: Yes
- Resting: No
- AFK: No
- Dead or ghost: No
- Timestamp: **Wed Feb 14 20:50:15 2024**

```lua
[ADDON_ACTION_BLOCKED] AddOn 'MUI_Core' tried to call the protected function 'MainMenuBarButtonContainer12:SetShown()'.
[string "../MUI_Core/Engine/Events/EventManager.lua"]:69: in function <...rface/AddOns/MUI_Core/Engine/Events/EventManager.lua:52>
[string "=[C]"]: in function `SetShown'
[string "@Interface/FrameXML/ActionBar.lua"]:198: in function `UpdateShownButtons'
[string "@Interface/FrameXML/ActionButton.lua"]:507: in function `UpdateAction'
[string "@Interface/FrameXML/ActionButton.lua"]:981: in function `OnEvent'
[string "@Interface/FrameXML/ActionButton.lua"]:207: in function <Interface/FrameXML/ActionButton.lua:204>
```
---
- Zone:  ()
- Group size: 0
- Instance type: none
- In combat: No
- Resting: Yes
- AFK: No
- Dead or ghost: No
- Timestamp: **Mon Feb 19 11:35:20 2024**

```lua
...e/AddOns/MUI_Core/Engine/Toolkit/Utilities/Other.lua:274: attempt to perform arithmetic on local 'itemLevel' (a nil value)
[string "../MUI_Core/Engine/Toolkit/Utilities/Other.lua"]:274: in function `GetInspectItemLevel'
[string "../MUI_Core/Modules/Tooltips/Tooltips.lua"]:886: in function <...erface/AddOns/MUI_Core/Modules/Tooltips/Tooltips.lua:870>
[string "../MUI_Core/Modules/Tooltips/Tooltips.lua"]:1279: in function <...erface/AddOns/MUI_Core/Modules/Tooltips/Tooltips.lua:1272>
[string "../MUI_Core/Modules/Tooltips/Tooltips.lua"]:1292: in function <...erface/AddOns/MUI_Core/Modules/Tooltips/Tooltips.lua:1290>
[string "=[C]"]: in function `securecallfunction'
[string "@Interface/SharedXML/Tooltip/TooltipDataHandler.lua"]:162: in function <Interface/SharedXML/Tooltip/TooltipDataHandler.lua:157>
[string "@Interface/SharedXML/Tooltip/TooltipDataHandler.lua"]:182: in function <Interface/SharedXML/Tooltip/TooltipDataHandler.lua:178>
[string "@Interface/SharedXML/Tooltip/TooltipDataHandler.lua"]:218: in function <Interface/SharedXML/Tooltip/TooltipDataHandler.lua:208>
[string "=[C]"]: in function `SetAttribute'
[string "@Interface/SharedXML/Tooltip/TooltipDataHandler.lua"]:243: in function <Interface/SharedXML/Tooltip/TooltipDataHandler.lua:236>
[string "@Interface/SharedXML/Tooltip/TooltipDataHandler.lua"]:389: in function <Interface/SharedXML/Tooltip/TooltipDataHandler.lua:339>
[string "=[C]"]: in function `securecallfunction'
[string "@Interface/SharedXML/Tooltip/TooltipDataHandler.lua"]:336: in function <Interface/SharedXML/Tooltip/TooltipDataHandler.lua:335>
[string "@Interface/FrameXML/UnitFram
```

### MUI_Core global settings
```lua
{["core"]={["setup"]={["addOns"]={["1"]={"..."},["2"]={"..."},["3"]={"..."},["4"]={"..."}}}},["DragonflightBarLayout_V2"]=true,["datatext"]={["money"]={["characters"]={["Calydal-Antonidas"]=148373924,["Arabellanix-Antonidas"]=316568723,["Basus-Antonidas"]=4127956378}}}}
```

### MUI_Core Current Profile Settings
```lua
{["installMessage"]="6.9.8",["actionbars"]={["bottom"]={["tutorial"]="6.9.8",["animation"]={["activeSets"]=2}}},["datatext"]={["money"]={["date"]="19-2",["todayMoney"]=148373924}},["unitPanels"]={["sufGradients"]={["to"]={["a"]=0,["b"]=0,["g"]=0,["r"]=0},["from"]={["a"]=0.5,["b"]=0.44705885648727,["g"]=0.82745105028152,["r"]=0.66666668653488}}},["chat"]={["highlighted"]={["1"]={["1"]="healers",["2"]="healer",["3"]="healz",["4"]="heals",["5"]="heal",["6"]="healing",["color"]={"..."},["sound"]=false,["upperCase"]=false},["2"]={["1"]="tanks",["2"]="tank",["3"]="tanking",["color"]={"..."},["sound"]=false,["upperCase"]=false},["3"]={["1"]="dps",["color"]={"..."},["sound"]=false,["upperCase"]=false},["4"]={["1"]="Calydal",["color"]={"..."},["sound"]=3081,["upperCase"]=false}}}}
```

### TimerBars Current Profile Settings
```lua
{["fieldNames"]={["1"]="Player",["2"]="Target"},["fields"]={["Target"]={["unitID"]="target",["position"]={["1"]="BOTTOMRIGHT",["2"]="MUI_TargetName",["3"]="TOPRIGHT",["4"]=-10,["5"]=2}},["Player"]={["unitID"]="player",["position"]={["1"]="BOTTOMLEFT",["2"]="MUI_PlayerName",["3"]="TOPLEFT",["4"]=12,["5"]=2}}}}
```

### Loaded AddOns
- <DBM Core> Main Core (2.06mb)
- <DBM Core> Status Bar Timers (89.9kb)
- <DBM Extra> Archaeology (7.2kb)
- <DBM Media> Voicepack VEM (0kb)
- Argent Gruntling & Argent Squire Silencer (0kb)
- Auctionator (3.28mb)
- BagBrother (35.6kb)
- Bagnon (1.33mb)
- Bartender4 (2.15mb)
- Details! Damage Meter (18.8mb)
- Details!: Compare 2.0 (97.2kb)
- Details!: Encounter Breakdown (plugin) (847.2kb)
- Details!: Raid Check (plugin) (75.4kb)
- Details!: Streamer (plugin) (163.8kb)
- Details!: Tiny Threat (plugin) (53.5kb)
- Details!: Vanguard (plugin) (68.2kb)
- HandyNotes (307.9kb)
- HandyNotes: Dragonflight (8.62mb)
- HandyNotes_DragonGlyphs (37.3kb)
- Leatrix Maps (643.1kb)
- Leatrix Plus (1.24mb)
- Masque (1.76mb)
- Masque: Caith (32.8kb)
- MayronUI Core (5.66mb)
- MayronUI Setup (366.1kb)
- OmniCC (114.1kb)
- Questie ShuptUp! (2.4kb)
- Shadowed Unit Frames (2.53mb)
- Titan Panel [_Core_] 8.0.5 (8.12mb)
- Titan Panel [Attributes] Multi! v6.3.2 (335kb)
- Titan Panel [Bag] 8.0.5 (34.8kb)
- Titan Panel [Clock] 8.0.5 (36.3kb)
- Titan Panel [Currencies] Multi! v9.20.0 (1.03mb)
- Titan Panel [Gold] 8.0.5 (59.7kb)
- Titan Panel [Location] 8.0.5 (123.7kb)
- Titan Panel [LootType] 8.00.0 (33.3kb)
- Titan Panel [Performance] 8.0.5 (48.7kb)
- Titan Panel [Professions] Multi! v9.2.9 (737.2kb)
- Titan Panel [Repair] 8.0.5 (86.7kb)
- Titan Panel [Spacer] v3.1.4 (57.7kb)
- Titan Panel [Volume] 8.0.5 (44.3kb)
- Titan Panel [XP] 8.0.5 (34.3kb)
- TomTom (1.79mb)### Bug Details
Ês können keine Plunderteile bei irgendeinen Hänler verkauft werden.

### Steps to Replicate
Schritt 1: k.A.
Schritt 2: k.A.
Schritt 3: k.A.

### MUI Version Info
- MUI_Core: 6.9.8
- MUI_Config: 6.9.8
- MUI_Setup: 6.9.8

### WoW Client Info
- WoW version: 10.2.5 (53262)
- Locale: deDE
- Resolution: 1920 (UI scale: 0.7)
- Using Mac: No

### Basic Character Info
- Faction: Alliance
- Class: Jäger (hunter)
- Specialization: Tierherrschaft
- Level: 64
- Race: Nachtelf

### Captured Errors (3)
- Zone: Drustvar (Gol Osigr)
- Group size: 0
- Instance type: none
- In combat: Yes
- Resting: No
- AFK: No
- Dead or ghost: No
- Timestamp: **Wed Feb 14 20:50:15 2024**

```lua
[ADDON_ACTION_BLOCKED] AddOn 'MUI_Core' tried to call the protected function 'ActionButton12:SetShown()'.
[string "../MUI_Core/Engine/Events/EventManager.lua"]:69: in function <...rface/AddOns/MUI_Core/Engine/Events/EventManager.lua:52>
[string "=[C]"]: in function `SetShown'
[string "@Interface/FrameXML/ActionBar.lua"]:195: in function `UpdateShownButtons'
[string "@Interface/FrameXML/ActionButton.lua"]:507: in function `UpdateAction'
[string "@Interface/FrameXML/ActionButton.lua"]:981: in function `OnEvent'
[string "@Interface/FrameXML/ActionButton.lua"]:207: in function <Interface/FrameXML/ActionButton.lua:204>
```
---
- Zone: Drustvar (Gol Osigr)
- Group size: 0
- Instance type: none
- In combat: Yes
- Resting: No
- AFK: No
- Dead or ghost: No
- Timestamp: **Wed Feb 14 20:50:15 2024**

```lua
[ADDON_ACTION_BLOCKED] AddOn 'MUI_Core' tried to call the protected function 'MainMenuBarButtonContainer12:SetShown()'.
[string "../MUI_Core/Engine/Events/EventManager.lua"]:69: in function <...rface/AddOns/MUI_Core/Engine/Events/EventManager.lua:52>
[string "=[C]"]: in function `SetShown'
[string "@Interface/FrameXML/ActionBar.lua"]:198: in function `UpdateShownButtons'
[string "@Interface/FrameXML/ActionButton.lua"]:507: in function `UpdateAction'
[string "@Interface/FrameXML/ActionButton.lua"]:981: in function `OnEvent'
[string "@Interface/FrameXML/ActionButton.lua"]:207: in function <Interface/FrameXML/ActionButton.lua:204>
```
---
- Zone:  ()
- Group size: 0
- Instance type: none
- In combat: No
- Resting: Yes
- AFK: No
- Dead or ghost: No
- Timestamp: **Mon Feb 19 11:35:20 2024**

```lua
...e/AddOns/MUI_Core/Engine/Toolkit/Utilities/Other.lua:274: attempt to perform arithmetic on local 'itemLevel' (a nil value)
[string "../MUI_Core/Engine/Toolkit/Utilities/Other.lua"]:274: in function `GetInspectItemLevel'
[string "../MUI_Core/Modules/Tooltips/Tooltips.lua"]:886: in function <...erface/AddOns/MUI_Core/Modules/Tooltips/Tooltips.lua:870>
[string "../MUI_Core/Modules/Tooltips/Tooltips.lua"]:1279: in function <...erface/AddOns/MUI_Core/Modules/Tooltips/Tooltips.lua:1272>
[string "../MUI_Core/Modules/Tooltips/Tooltips.lua"]:1292: in function <...erface/AddOns/MUI_Core/Modules/Tooltips/Tooltips.lua:1290>
[string "=[C]"]: in function `securecallfunction'
[string "@Interface/SharedXML/Tooltip/TooltipDataHandler.lua"]:162: in function <Interface/SharedXML/Tooltip/TooltipDataHandler.lua:157>
[string "@Interface/SharedXML/Tooltip/TooltipDataHandler.lua"]:182: in function <Interface/SharedXML/Tooltip/TooltipDataHandler.lua:178>
[string "@Interface/SharedXML/Tooltip/TooltipDataHandler.lua"]:218: in function <Interface/SharedXML/Tooltip/TooltipDataHandler.lua:208>
[string "=[C]"]: in function `SetAttribute'
[string "@Interface/SharedXML/Tooltip/TooltipDataHandler.lua"]:243: in function <Interface/SharedXML/Tooltip/TooltipDataHandler.lua:236>
[string "@Interface/SharedXML/Tooltip/TooltipDataHandler.lua"]:389: in function <Interface/SharedXML/Tooltip/TooltipDataHandler.lua:339>
[string "=[C]"]: in function `securecallfunction'
[string "@Interface/SharedXML/Tooltip/TooltipDataHandler.lua"]:336: in function <Interface/SharedXML/Tooltip/TooltipDataHandler.lua:335>
[string "@Interface/FrameXML/UnitFram
```

### MUI_Core global settings
```lua
{["core"]={["setup"]={["addOns"]={["1"]={"..."},["2"]={"..."},["3"]={"..."},["4"]={"..."}}}},["DragonflightBarLayout_V2"]=true,["datatext"]={["money"]={["characters"]={["Calydal-Antonidas"]=148373924,["Arabellanix-Antonidas"]=316568723,["Basus-Antonidas"]=4127956378}}}}
```

### MUI_Core Current Profile Settings
```lua
{["installMessage"]="6.9.8",["actionbars"]={["bottom"]={["tutorial"]="6.9.8",["animation"]={["activeSets"]=2}}},["datatext"]={["money"]={["date"]="19-2",["todayMoney"]=148373924}},["unitPanels"]={["sufGradients"]={["to"]={["a"]=0,["b"]=0,["g"]=0,["r"]=0},["from"]={["a"]=0.5,["b"]=0.44705885648727,["g"]=0.82745105028152,["r"]=0.66666668653488}}},["chat"]={["highlighted"]={["1"]={["1"]="healers",["2"]="healer",["3"]="healz",["4"]="heals",["5"]="heal",["6"]="healing",["color"]={"..."},["sound"]=false,["upperCase"]=false},["2"]={["1"]="tanks",["2"]="tank",["3"]="tanking",["color"]={"..."},["sound"]=false,["upperCase"]=false},["3"]={["1"]="dps",["color"]={"..."},["sound"]=false,["upperCase"]=false},["4"]={["1"]="Calydal",["color"]={"..."},["sound"]=3081,["upperCase"]=false}}}}
```

### TimerBars Current Profile Settings
```lua
{["fieldNames"]={["1"]="Player",["2"]="Target"},["fields"]={["Target"]={["unitID"]="target",["position"]={["1"]="BOTTOMRIGHT",["2"]="MUI_TargetName",["3"]="TOPRIGHT",["4"]=-10,["5"]=2}},["Player"]={["unitID"]="player",["position"]={["1"]="BOTTOMLEFT",["2"]="MUI_PlayerName",["3"]="TOPLEFT",["4"]=12,["5"]=2}}}}
```

### Loaded AddOns
- <DBM Core> Main Core (2.06mb)
- <DBM Core> Status Bar Timers (89.9kb)
- <DBM Extra> Archaeology (7.2kb)
- <DBM Media> Voicepack VEM (0kb)
- Argent Gruntling & Argent Squire Silencer (0kb)
- Auctionator (3.28mb)
- BagBrother (35.6kb)
- Bagnon (1.33mb)
- Bartender4 (2.15mb)
- Details! Damage Meter (18.8mb)
- Details!: Compare 2.0 (97.2kb)
- Details!: Encounter Breakdown (plugin) (847.2kb)
- Details!: Raid Check (plugin) (75.4kb)
- Details!: Streamer (plugin) (163.8kb)
- Details!: Tiny Threat (plugin) (53.5kb)
- Details!: Vanguard (plugin) (68.2kb)
- HandyNotes (307.9kb)
- HandyNotes: Dragonflight (8.62mb)
- HandyNotes_DragonGlyphs (37.3kb)
- Leatrix Maps (643.1kb)
- Leatrix Plus (1.24mb)
- Masque (1.76mb)
- Masque: Caith (32.8kb)
- MayronUI Core (5.66mb)
- MayronUI Setup (366.1kb)
- OmniCC (114.1kb)
- Questie ShuptUp! (2.4kb)
- Shadowed Unit Frames (2.53mb)
- Titan Panel [_Core_] 8.0.5 (8.12mb)
- Titan Panel [Attributes] Multi! v6.3.2 (335kb)
- Titan Panel [Bag] 8.0.5 (34.8kb)
- Titan Panel [Clock] 8.0.5 (36.3kb)
- Titan Panel [Currencies] Multi! v9.20.0 (1.03mb)
- Titan Panel [Gold] 8.0.5 (59.7kb)
- Titan Panel [Location] 8.0.5 (123.7kb)
- Titan Panel [LootType] 8.00.0 (33.3kb)
- Titan Panel [Performance] 8.0.5 (48.7kb)
- Titan Panel [Professions] Multi! v9.2.9 (737.2kb)
- Titan Panel [Repair] 8.0.5 (86.7kb)
- Titan Panel [Spacer] v3.1.4 (57.7kb)
- Titan Panel [Volume] 8.0.5 (44.3kb)
- Titan Panel [XP] 8.0.5 (34.3kb)
- TomTom (1.79mb)### Bug Details
Ês können keine Plunderteile bei irgendeinen Hänler verkauft werden.

### Steps to Replicate
Schritt 1: k.A.
Schritt 2: k.A.
Schritt 3: k.A.

### MUI Version Info
- MUI_Core: 6.9.8
- MUI_Config: 6.9.8
- MUI_Setup: 6.9.8

### WoW Client Info
- WoW version: 10.2.5 (53262)
- Locale: deDE
- Resolution: 1920 (UI scale: 0.7)
- Using Mac: No

### Basic Character Info
- Faction: Alliance
- Class: Jäger (hunter)
- Specialization: Tierherrschaft
- Level: 64
- Race: Nachtelf

### Captured Errors (3)
- Zone: Drustvar (Gol Osigr)
- Group size: 0
- Instance type: none
- In combat: Yes
- Resting: No
- AFK: No
- Dead or ghost: No
- Timestamp: **Wed Feb 14 20:50:15 2024**

```lua
[ADDON_ACTION_BLOCKED] AddOn 'MUI_Core' tried to call the protected function 'ActionButton12:SetShown()'.
[string "../MUI_Core/Engine/Events/EventManager.lua"]:69: in function <...rface/AddOns/MUI_Core/Engine/Events/EventManager.lua:52>
[string "=[C]"]: in function `SetShown'
[string "@Interface/FrameXML/ActionBar.lua"]:195: in function `UpdateShownButtons'
[string "@Interface/FrameXML/ActionButton.lua"]:507: in function `UpdateAction'
[string "@Interface/FrameXML/ActionButton.lua"]:981: in function `OnEvent'
[string "@Interface/FrameXML/ActionButton.lua"]:207: in function <Interface/FrameXML/ActionButton.lua:204>
```
---
- Zone: Drustvar (Gol Osigr)
- Group size: 0
- Instance type: none
- In combat: Yes
- Resting: No
- AFK: No
- Dead or ghost: No
- Timestamp: **Wed Feb 14 20:50:15 2024**

```lua
[ADDON_ACTION_BLOCKED] AddOn 'MUI_Core' tried to call the protected function 'MainMenuBarButtonContainer12:SetShown()'.
[string "../MUI_Core/Engine/Events/EventManager.lua"]:69: in function <...rface/AddOns/MUI_Core/Engine/Events/EventManager.lua:52>
[string "=[C]"]: in function `SetShown'
[string "@Interface/FrameXML/ActionBar.lua"]:198: in function `UpdateShownButtons'
[string "@Interface/FrameXML/ActionButton.lua"]:507: in function `UpdateAction'
[string "@Interface/FrameXML/ActionButton.lua"]:981: in function `OnEvent'
[string "@Interface/FrameXML/ActionButton.lua"]:207: in function <Interface/FrameXML/ActionButton.lua:204>
```
---
- Zone:  ()
- Group size: 0
- Instance type: none
- In combat: No
- Resting: Yes
- AFK: No
- Dead or ghost: No
- Timestamp: **Mon Feb 19 11:35:20 2024**

```lua
...e/AddOns/MUI_Core/Engine/Toolkit/Utilities/Other.lua:274: attempt to perform arithmetic on local 'itemLevel' (a nil value)
[string "../MUI_Core/Engine/Toolkit/Utilities/Other.lua"]:274: in function `GetInspectItemLevel'
[string "../MUI_Core/Modules/Tooltips/Tooltips.lua"]:886: in function <...erface/AddOns/MUI_Core/Modules/Tooltips/Tooltips.lua:870>
[string "../MUI_Core/Modules/Tooltips/Tooltips.lua"]:1279: in function <...erface/AddOns/MUI_Core/Modules/Tooltips/Tooltips.lua:1272>
[string "../MUI_Core/Modules/Tooltips/Tooltips.lua"]:1292: in function <...erface/AddOns/MUI_Core/Modules/Tooltips/Tooltips.lua:1290>
[string "=[C]"]: in function `securecallfunction'
[string "@Interface/SharedXML/Tooltip/TooltipDataHandler.lua"]:162: in function <Interface/SharedXML/Tooltip/TooltipDataHandler.lua:157>
[string "@Interface/SharedXML/Tooltip/TooltipDataHandler.lua"]:182: in function <Interface/SharedXML/Tooltip/TooltipDataHandler.lua:178>
[string "@Interface/SharedXML/Tooltip/TooltipDataHandler.lua"]:218: in function <Interface/SharedXML/Tooltip/TooltipDataHandler.lua:208>
[string "=[C]"]: in function `SetAttribute'
[string "@Interface/SharedXML/Tooltip/TooltipDataHandler.lua"]:243: in function <Interface/SharedXML/Tooltip/TooltipDataHandler.lua:236>
[string "@Interface/SharedXML/Tooltip/TooltipDataHandler.lua"]:389: in function <Interface/SharedXML/Tooltip/TooltipDataHandler.lua:339>
[string "=[C]"]: in function `securecallfunction'
[string "@Interface/SharedXML/Tooltip/TooltipDataHandler.lua"]:336: in function <Interface/SharedXML/Tooltip/TooltipDataHandler.lua:335>
[string "@Interface/FrameXML/UnitFram
```

### MUI_Core global settings
```lua
{["core"]={["setup"]={["addOns"]={["1"]={"..."},["2"]={"..."},["3"]={"..."},["4"]={"..."}}}},["DragonflightBarLayout_V2"]=true,["datatext"]={["money"]={["characters"]={["Calydal-Antonidas"]=148373924,["Arabellanix-Antonidas"]=316568723,["Basus-Antonidas"]=4127956378}}}}
```

### MUI_Core Current Profile Settings
```lua
{["installMessage"]="6.9.8",["actionbars"]={["bottom"]={["tutorial"]="6.9.8",["animation"]={["activeSets"]=2}}},["datatext"]={["money"]={["date"]="19-2",["todayMoney"]=148373924}},["unitPanels"]={["sufGradients"]={["to"]={["a"]=0,["b"]=0,["g"]=0,["r"]=0},["from"]={["a"]=0.5,["b"]=0.44705885648727,["g"]=0.82745105028152,["r"]=0.66666668653488}}},["chat"]={["highlighted"]={["1"]={["1"]="healers",["2"]="healer",["3"]="healz",["4"]="heals",["5"]="heal",["6"]="healing",["color"]={"..."},["sound"]=false,["upperCase"]=false},["2"]={["1"]="tanks",["2"]="tank",["3"]="tanking",["color"]={"..."},["sound"]=false,["upperCase"]=false},["3"]={["1"]="dps",["color"]={"..."},["sound"]=false,["upperCase"]=false},["4"]={["1"]="Calydal",["color"]={"..."},["sound"]=3081,["upperCase"]=false}}}}
```

### TimerBars Current Profile Settings
```lua
{["fieldNames"]={["1"]="Player",["2"]="Target"},["fields"]={["Target"]={["unitID"]="target",["position"]={["1"]="BOTTOMRIGHT",["2"]="MUI_TargetName",["3"]="TOPRIGHT",["4"]=-10,["5"]=2}},["Player"]={["unitID"]="player",["position"]={["1"]="BOTTOMLEFT",["2"]="MUI_PlayerName",["3"]="TOPLEFT",["4"]=12,["5"]=2}}}}
```

### Loaded AddOns
- <DBM Core> Main Core (2.06mb)
- <DBM Core> Status Bar Timers (89.9kb)
- <DBM Extra> Archaeology (7.2kb)
- <DBM Media> Voicepack VEM (0kb)
- Argent Gruntling & Argent Squire Silencer (0kb)
- Auctionator (3.28mb)
- BagBrother (35.6kb)
- Bagnon (1.33mb)
- Bartender4 (2.15mb)
- Details! Damage Meter (18.8mb)
- Details!: Compare 2.0 (97.2kb)
- Details!: Encounter Breakdown (plugin) (847.2kb)
- Details!: Raid Check (plugin) (75.4kb)
- Details!: Streamer (plugin) (163.8kb)
- Details!: Tiny Threat (plugin) (53.5kb)
- Details!: Vanguard (plugin) (68.2kb)
- HandyNotes (307.9kb)
- HandyNotes: Dragonflight (8.62mb)
- HandyNotes_DragonGlyphs (37.3kb)
- Leatrix Maps (643.1kb)
- Leatrix Plus (1.24mb)
- Masque (1.76mb)
- Masque: Caith (32.8kb)
- MayronUI Core (5.66mb)
- MayronUI Setup (366.1kb)
- OmniCC (114.1kb)
- Questie ShuptUp! (2.4kb)
- Shadowed Unit Frames (2.53mb)
- Titan Panel [_Core_] 8.0.5 (8.12mb)
- Titan Panel [Attributes] Multi! v6.3.2 (335kb)
- Titan Panel [Bag] 8.0.5 (34.8kb)
- Titan Panel [Clock] 8.0.5 (36.3kb)
- Titan Panel [Currencies] Multi! v9.20.0 (1.03mb)
- Titan Panel [Gold] 8.0.5 (59.7kb)
- Titan Panel [Location] 8.0.5 (123.7kb)
- Titan Panel [LootType] 8.00.0 (33.3kb)
- Titan Panel [Performance] 8.0.5 (48.7kb)
- Titan Panel [Professions] Multi! v9.2.9 (737.2kb)
- Titan Panel [Repair] 8.0.5 (86.7kb)
- Titan Panel [Spacer] v3.1.4 (57.7kb)
- Titan Panel [Volume] 8.0.5 (44.3kb)
- Titan Panel [XP] 8.0.5 (34.3kb)
- TomTom (1.79mb)
