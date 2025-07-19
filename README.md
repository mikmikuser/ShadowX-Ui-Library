# 🌌 ShadowX UI Library

ShadowX is a glowing, Fluent-inspired Roblox UI library designed for both **Mobile** and **PC**. Created by **MBR DEV**, this library provides a clean and powerful interface with buttons, toggles, sliders, dropdowns, inputs, keybinds, and more.

> ✨ Modern UI • 📱 Mobile Friendly • ⚙️ Developer Ready

---

## 📦 Installation

To load the library directly from your GitHub repository:

```lua
-- Load the live library from your GitHub source
local ShadowX = loadstring(game:HttpGet("https://raw.githubusercontent.com/mikmikuser/ShadowX-Ui-Library/main/ShadowXLib.lua"))()
```

---

## 🚀 Getting Started

Create your main UI window and tab:

```lua
local Window = ShadowX:CreateWindow({
    Title = "ShadowX Hub",
    SubTitle = "By MBR DEV",
    TabWidth = 100,
    Size = UDim2.new(0, 420, 0, 360),
    Theme = "Dark"
})

local MainTab = Window:AddTab("Main")
```

---

## ✨ Features & Usage

### 🔘 AddButton

```lua
MainTab:AddButton("Click Me", function()
    print("Button Clicked!")
end)
```

### 🔄 AddToggle

```lua
MainTab:AddToggle("Enable Feature", false, function(state)
    print("Toggle State:", state)
end)
```

### 🎚️ AddSlider

```lua
MainTab:AddSlider("Volume", 0, 100, 50, function(value)
    print("Slider Value:", value)
end)
```

### 🔽 AddDropdown

```lua
MainTab:AddDropdown("Choose Option", {"Option 1", "Option 2"}, function(selected)
    print("Selected Option:", selected)
end)
```

### ⌨️ AddInput

```lua
MainTab:AddInput("Enter Text", function(input)
    print("Input:", input)
end)
```

### 🎮 AddKeybind

```lua
MainTab:AddKeybind("Toggle UI", Enum.KeyCode.RightControl, function()
    Window:Toggle()
end)
```

---

## 🧱 Full Example

Here’s a full example putting everything together:

```lua
local ShadowX = loadstring(game:HttpGet("https://raw.githubusercontent.com/YOUR-USERNAME/ShadowX/main/ShadowXLib.lua"))()

local Window = ShadowX:CreateWindow({
    Title = "ShadowX Hub",
    SubTitle = "By MBR DEV",
    TabWidth = 100,
    Size = UDim2.new(0, 420, 0, 360),
    Theme = "Dark"
})

local MainTab = Window:AddTab("Main")

MainTab:AddButton("Click Me", function()
    print("Button Pressed!")
end)

MainTab:AddToggle("Auto Mode", true, function(state)
    print("Auto Mode:", state)
end)

MainTab:AddSlider("Speed", 0, 100, 20, function(speed)
    print("Speed:", speed)
end)

MainTab:AddDropdown("Choose Option", {"A", "B", "C"}, function(selected)
    print("Option:", selected)
end)

MainTab:AddInput("Enter something", function(txt)
    print("Input was:", txt)
end)

MainTab:AddKeybind("Right Control", Enum.KeyCode.RightControl, function()
    Window:Toggle()
end)
```

---

## 🌐 Hosting Remotely on GitHub

To make ShadowX loadable remotely:

1. Create a GitHub repository (e.g. `ShadowX`)
2. Upload your `ShadowXLib.lua`
3. Use:

```lua
loadstring(game:HttpGet("https://raw.githubusercontent.com/YOUR-USERNAME/ShadowX/main/ShadowXLib.lua"))()
```

---

## 📁 Library Structure

```
ShadowX/
├── ShadowXLib.lua
└── README.md
```

---

## 🧑‍💻 Author

Made with 💙 by **MBR DEV**  
Custom UI Design for Mobile and PC Roblox Scripts.

---

## 📜 License

MIT License — Free to use, fork, and modify.  
Credit is appreciated when using this library in public scripts.

---
