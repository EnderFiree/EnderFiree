local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()
local Player = game.Players.LocalPlayer

local Window =
OrionLib:MakeWindow({Name = "Key System", HidePremium = false, SaveConfig = true, IntroEnabled = false})


_G.Key = "Hdidbsnonimapnoe982"
_G.KeyInput = "string"

function MakeScriptHub()
     local Window =
OrionLib:MakeWindow({Name = "OrionLib | Hub", HidePremium = false, SaveConfig = true, IntroEnabled = false})

















	



local Tab = Window:MakeTab({
	Name = "Key",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

Tab:AddTextbox({
	Name = "Enter Key",
	Default = "",
	TextDisappear = true,
	Callback = function(Value)
		_G.KeyInput = Value
	end	  
})

Tab:AddButton({
	Name = "Check Key",
	Callback = function()
      		if _G.KeyInput == _G.Key then 
					MakeScriptHub()
					end
  	end    
})





OrionLib:Init()
