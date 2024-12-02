local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()
local Window = OrionLib:MakeWindow({Name = "Orion | Hub", HidePremium = true, SaveConfig = true, ConfigFolder = "OrionTest"})
local Tab = Window:MakeTab({
	Name = "Blox Fruits",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = true
})
Tab:AddButton({
	Name = "Neva Hub {OP}",
	Callback = function()
      		loadstring(game:HttpGet('https://raw.githubusercontent.com/VEZ2/NEVAHUB/main/2'))()
  	end    
})
local Tab = Window:MakeTab({
	Name = "Strongest Battleground",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = true
})
Tab:AddButton({
	Name = "Auto Kyoto {NEW}",
	Callback = function()
	                    loadstring(game:HttpGet("https://pastebin.com/raw/q8Y2a836"))()
		 end
})
local Tab = Window:MakeTab({
	Name = "Universal",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = true
})
Tab:AddButton({
	Name = "Chat Admin Script {TROLL}",
	Callback = function()
	               loadstring(game:HttpGet("https://raw.githubusercontent.com/game-hax/uca/main/release/uca.min.lua"))()
			end
})
Tab:AddButton({
	Name = "Infinite Yield {OP}",
	Callback = function()
	               loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'))()
			end
})
local Tab = Window:MakeTab({
	Name = "Blade Ball",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = true
	})
Tab:AddButton({
	Name = "Hub BB {OP}",
	Callback = function()
	           loadstring(game:HttpGet("https://raw.githubusercontent.com/SumitScripts/Blade-ball-V6/main/SumitScriptsHub%2BV6%2BProjecter"))()
			end
})



OrionLib:Init()
