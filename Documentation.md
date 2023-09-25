# LuxWare User Interface
Unofficial (kinda idk because im the first to release a doc) document on this.
Everything Works For Mobile Btw Js Not The Slider
# Getting The Loadstring
```lua
local Luxtl = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Luxware-UI-Library/main/Source.lua"))()
```
# Creating a Window
```lua
local Luxt = Luxtl.CreateWindow("Tutorial", Image)
```
## Creating Tabs
```lua
local mainTab = Luxt:Tab("Main", Image)
```
## Creating Sections
```lua
local section = mainTab:Section("Section")
```
## Creating Labels
```lua
section:Label("Label")
```
### Creating Buttons
```lua
section:Button("Button", function()
    print("Clicked!")
end)
```
### Creating Toggles
```lua
section:Toggle("Toggle", function(Value)
    print(Value)
end)
```
### Creating TextBoxes
```lua
section:TextBox("TextBox", "PlaceHolder", function(Value)
    print(Value)
end)
```
### Creating Sliders
Sadly Buggy On Mobile
```lua
section:Slider("Slider", 0 -- Lowest Number And Default, 1000 -- Max Number, function(Value)
    print(Value)
end)
```
### Creating DropDowns
```lua
section:DropDown("DropDown", {"Option 1", "Option 2", "Option 3"}, function(Value) 
    print(Value)
end)
```
