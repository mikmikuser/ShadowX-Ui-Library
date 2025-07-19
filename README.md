
### 🔘 CreateWindow

```lua
local Window = ShadowX:CreateWindow({
    Title = "ShadowX Hub",
    SubTitle = "Made by MBR DEV",
    TabWidth = 100,
    Size = UDim2.new(0, 420, 0, 360),
    Theme = "Dark"
})



### 🗂️ AddTab

local MainTab = Window:AddTab("Main")



### 🖱️ AddButton

MainTab:AddButton("Click Me", function()
    print("Button Clicked!")
end)


### 🔄 AddToggle

MainTab:AddToggle("Enable Feature", false, function(state)
    print("Toggle is", state)
end)


### 🎚️ AddSlider

MainTab:AddSlider("Adjust Value", 0, 100, 50, function(value)
    print("Slider Value:", value)
end)



### 🔽 AddDropdown

MainTab:AddDropdown("Choose Option", {"Option 1", "Option 2", "Option 3"}, function(selected)
    print("Selected:", selected)
end)



### ⌨️ AddInput

MainTab:AddInput("Enter Text", function(text)
    print("Input Received:", text)
end)



### 🎮 AddKeybind

MainTab:AddKeybind("Toggle UI", Enum.KeyCode.RightControl, function()
    Window:Toggle()
end)
