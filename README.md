local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()
local Window = OrionLib:MakeWindow({Name = "Key System", HidePremium = false, SaveConfig = true, ConfigFolder = "OrionTest"})

_G.Key = "Sytjahdjamhrowovbk972hk"
_G.KeyInput = "string"

local Tab = Window:MakeTab({
	Name = "Key",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

_G.Key = "Sytjahdjamhrowovbk972hk"
_G.KeyInput = "string"

Tab:AddTextbox({
	Name = "Enter Key",
	Default = "",
	TextDisappear = true,
	Callback = function(Value)
	end	  
})



Tab:AddButton({
	Name = "Check Key",
	Callback = function()
	        MakeScriptHub()
local Window = OrionLib:MakeWindow({Name = "OrionLib | Hub", HidePremium = false, SaveConfig = true, ConfigFolder = "Orion"})







OrionLib:Init()
