---
title: Binds
sidebar_position: 2
image: /img/arrayfield/arrayfieldbg.jpg
description: How to create keybinds
---

# Binding keys in ArrayField

## Creating a Keybind

```lua
local Keybind = Tab:CreateKeybind({
   Name = "Keybind Example",
   CurrentKeybind = "Q",
   HoldToInteract = false,
   Flag = "Keybind1", -- A flag is the identifier for the configuration file, make sure every element has a different flag if you're using configuration saving to ensure no overlaps
   Callback = function(Keybind)
   -- The function that takes place when the keybind is pressed
   -- The variable (Keybind) is a boolean for whether the keybind is being held or not (HoldToInteract needs to be true)
   end,
})
```

### Updating a Keybind

```lua
Keybind:Set("RightCtrl") -- Keybind (string)
```
