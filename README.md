local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()
local Window =
OrionLib:MakeWindow({Name = "Key System", HidePremium = false, SaveConfig = true, IntroEnabled = false})


_G.Key = "Hdidbsnonimapnoe982"
_G.KeyInput = "string"



local Tab = Window:MakeTab({
	Name = "Key",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

Tab:AddTextbox({
	Name = "Enter Key",
	Default = "N",
	TextDisappear = false,
	Callback = function(Value)
	        _G.Key  _G.KeyInput
	   end	  
})

Tab:AddButton({
	Name = "Check Key"
  Callback = function()
      		_G.Key _G.KeyInput










OrionLib:Init()
