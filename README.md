# creating library:

```luau
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/CoolManYesYes/Kr4k/refs/heads/main/LibReCoded.lua"))()
```

# creating window:

```luau
local Window = Library.Window('KR4K Library')
```

# creating tab:

```luau
local Test1 = Window.CreateTab('Welcome!')
```

# creating dividers:

```luau
Test1.CreateDivider("Im a divider!")
```

# creating labels:

```luau
Test1.CreateLabel("i love being a label!")
```

# creating buttons:

```luau
Test1.CreateButton("Click me!", function()
	print("Yay! I got clicked!")
end)
```

# creating sliders:

```luau
Test1.CreateSlider("Print", 0, 50, function(s)
	print(s)
end)
```

# creating keybinds:

```luau
Test1.CreateKeybind("Print on key!", Enum.KeyCode.F, function()
	print("I'm a keybind!")
end)
```

# toggling ui with keybinds:

```luau
Test1.CreateKeybind("Toggle UI", Enum.KeyCode.RightAlt, function()
	Library:ToggleUI()
end)
```
