local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()

-- Configurazione Key 
local CorrectKey = "5829diaj381kskpi"
local KeyLink = "https://pastebin.com/xpNHZRzq" -- Sostituisci con un link reale

-- Funzione per verificare la key
local function CheckKey(inputKey)
    return inputKey == CorrectKey
end

-- Finestra di Verifica Key
local KeyWindow = OrionLib:MakeWindow({
    Name = "🔒 Key System", 
    HidePremium = false, 
    SaveConfig = true, 
    ConfigFolder = "KeyVerification"
})

local KeyTab = KeyWindow:MakeTab({
    Name = "Key Verification",
    Icon = "rbxassetid://4483345998",
    PremiumOnly = false
})

-- Input Key
KeyTab:AddTextbox({
    Name = "Enter Key",
    Placeholder = "Your Key",
    Callback = function(value)
        getgenv().UserKey = value
    end    
})

-- Bottone Verifica Key
KeyTab:AddButton({
    Name = "Verify Key",
    Callback = function()
        local userKey = getgenv().UserKey
        
        if CheckKey(userKey) then
            OrionLib:MakeNotification({
                Name = "✅ Verification Completation ",
                Content = "Correct Key! Loading script...",
                Image = "rbxassetid://4483345998",
                Time = 3
            })
            
            
            wait(2)
            OrionLib:Destroy()
              
            local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()
local Window = OrionLib:MakeWindow({Name = "OrionLib | Hub", HidePremium = false, SaveConfig = true, ConfigFolder = "Orion"})
local Tab = Window:MakeTab({
	Name = "Blox Fruits",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})
Tab:AddButton({
	Name = "Speed Hub {DRAGON REWORK}",
	Callback = function()
      		loadstring(game:HttpGet("https://raw.githubusercontent.com/AhmadV99/Speed-Hub-X/main/Speed%20Hub%20X.lua", true))()
  	end    
})


local Tab = Window:MakeTab({
	Name = "Universal",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})
Tab:AddButton({
	Name = "Infinite Yield {OP}",
	Callback = function()
          loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'))()
        end
})



Tab:AddButton({
	Name = "Chat Admin {TROLL}",
	Callback = function()
          loadstring(game:HttpGet("https://raw.githubusercontent.com/game-hax/uca/main/release/uca.min.lua"))()
      end
})




Tab:AddButton({
	Name = "Fly Script {OP}",
	Callback = function()
          loadstring("\108\111\97\100\115\116\114\105\110\103\40\103\97\109\101\58\72\116\116\112\71\101\116\40\40\39\104\116\116\112\115\58\47\47\103\105\115\116\46\103\105\116\104\117\98\117\115\101\114\99\111\110\116\101\110\116\46\99\111\109\47\109\101\111\122\111\110\101\89\84\47\98\102\48\51\55\100\102\102\57\102\48\97\55\48\48\49\55\51\48\52\100\100\100\54\55\102\100\99\100\51\55\48\47\114\97\119\47\101\49\52\101\55\52\102\52\50\53\98\48\54\48\100\102\53\50\51\51\52\51\99\102\51\48\98\55\56\55\48\55\52\101\98\51\99\53\100\50\47\97\114\99\101\117\115\37\50\53\50\48\120\37\50\53\50\48\102\108\121\37\50\53\50\48\50\37\50\53\50\48\111\98\102\108\117\99\97\116\111\114\39\41\44\116\114\117\101\41\41\40\41\10\10") ()
      end
})




local Tab = Window:MakeTab({
	Name = "Blade Ball",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})
Tab:AddButton({
	Name = "Hub BB {OP}",
	Callback = function()
          loadstring(game:HttpGet("https://raw.githubusercontent.com/redopy7/Blade-Ball/refs/heads/main/Kalitor"))()
       end
})




local Tab = Window:MakeTab({
	Name = "Strongest Bt",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})
Tab:AddButton({
	Name = "Auto Kyoto {OP}",
	Callback = function()
          loadstring(game:HttpGet("https://paste bin.com/raw/q8Y2a836"))()
        end
})




local Tab = Window:MakeTab({
	Name = "Fisch",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})
Tab:AddButton({
	Name = "SpeedHub {OP}",
	Callback = function()
      loadstring(game:HttpGet("https://raw.githubusercontent.com/AhmadV99/Speed-Hub-X/main/Speed%20Hub%20X.lua", true))()
  	end    
})
local Tab = Window:MakeTab({
	Name = "Funky Friday",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})
Tab:AddButton({
	Name = "Funky Friday Hub{OP}",
	Callback = function()
      loadstring(game:HttpGet('https://pastebin.com/raw/dcyuEgyK'))()
			end
})


local Tab = Window:MakeTab({
	Name = "Rivals",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})
Tab:AddButton({
	Name = " Neutron Hub{OP}",
	Callback = function()
           loadstring(game:HttpGet("https://raw.githubusercontent.com/PawsThePaw/Neutron.lua/refs/heads/main/V1.0.2.txt", true))();
			 end
})

local Tab = Window:MakeTab({
	Name = "Aut",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})
Tab:AddButton({
	Name = " Demonic Hub{NEW}",
	Callback = function()
           loadstring(game:HttpGet("https://raw.githubusercontent.com/OhhMyGehlee/Mul/refs/heads/main/ver"))()
			 end
})

local Tab = Window:MakeTab({
	Name = "Sols rng",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})
Tab:AddButton({
	Name = " Erudite Hub{NEW}",
	Callback = function()
           loadstring(game:HttpGet("https://raw.githubusercontent.com/ThacG/EruditeHub/main/Sol's%20RNG/V2.69"))()
			 end
})

local Tab = Window:MakeTab({
	Name = "Veichle Legends",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})
Tab:AddButton({
	Name = " Vesta Hub{NEW}",
	Callback = function()
    
loadstring(game:HttpGet("https://raw.githubusercontent.com/Marco8642/science/main/Vehicle%20legends"))()
         end
})














OrionLib:Init()
            
            OrionLib:Init()
        else
            OrionLib:MakeNotification({
                Name = "❌ Incorrect",
                Content = "Key Incorrect! Try.",
                Image = "rbxassetid://4483345998",
                Time = 3
            })
        end
    end
})

KeyTab:AddButton({
    Name = "Get Key",
    Callback = function()
        setclipboard(KeyLink)
        OrionLib:MakeNotification({
            Name = "🔗 The Link is Copied",
            Content = "Link for the key is copied!",
            Image = "rbxassetid://4483345998",
            Time = 3
        })
    end
})

OrionLib:Init()