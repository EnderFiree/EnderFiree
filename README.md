local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()

-- Key Configuration
local CorrectKey = "5829diaj381kskpi"
local KeyLink = "https://pastebin.com/xpNHZRzq" -- Replace with a real link
local ConfigFolder = "KeyVerification" -- Folder for saving

-- Function to verify the key
local function CheckKey(inputKey)
    return inputKey == CorrectKey
end

-- Function to save the Key
local function SaveKey(key)
    if not isfolder(ConfigFolder) then
        makefolder(ConfigFolder)
    end
    writefile(ConfigFolder .. "/SavedKey.txt", key)
end

-- Function to load saved Key
local function LoadKey()
    if isfile(ConfigFolder .. "/SavedKey.txt") then
        return readfile(ConfigFolder .. "/SavedKey.txt")
    else
        return nil
    end
end

-- Load saved Key
local SavedKey = LoadKey()

-- Key Verification Window
local KeyWindow = OrionLib:MakeWindow({
    Name = "🔒 Key System",
    HidePremium = false,
    SaveConfig = true,
    ConfigFolder = ConfigFolder
})

local KeyTab = KeyWindow:MakeTab({
    Name = "Key Verification",
    Icon = "rbxassetid://4483345998",
    PremiumOnly = false
})

-- Key Input
KeyTab:AddTextbox({
    Name = "Enter Key",
    Default = SavedKey or "", -- Show saved Key if available
    Placeholder = "Your Key",
    Callback = function(value)
        getgenv().UserKey = value
    end    
})

-- Key Verification Button
KeyTab:AddButton({
    Name = "Verify Key",
    Callback = function()
        local userKey = getgenv().UserKey

        if CheckKey(userKey) then
            -- Save correct Key
            SaveKey(userKey)

            OrionLib:MakeNotification({
                Name = "✅ Verification Completed",
                Content = "Correct Key! Loading script...",
                Image = "rbxassetid://4483345998",
                Time = 3
            })

            wait(2)
            OrionLib:Destroy()

            -- Open main system
            local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()
            local Window = OrionLib:MakeWindow({Name = "OrionLib | Hub", HidePremium = false, SaveConfig = true, ConfigFolder = "Orion"})

            -- Blox Fruits Section
            local Tab = Window:MakeTab({
                Name = "Blox Fruits",
                Icon = "rbxassetid://4483345998",
                PremiumOnly = false
            })
            Tab:AddButton({
                Name = "HoHo Hub {MOBILE}",
                Callback = function()
                    loadstring(game:HttpGet("https://raw.githubusercontent.com/acsu123/HOHO_H/main/Loading_UI"))()
                end    
            })

            -- Universal Section
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
                    loadstring(game:HttpGet("https://gist.githubusercontent.com/meozoneYT/000/raw/fly.lua"))()
                end
            })

            -- Blade Ball Section
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

            -- Strongest Battlegrounds Section
            local Tab = Window:MakeTab({
                Name = "Strongest Bt",
                Icon = "rbxassetid://4483345998",
                PremiumOnly = false
            })
            Tab:AddButton({
                Name = "Auto Kyoto {OP}",
                Callback = function()
                    loadstring(game:HttpGet("https://pastebin.com/raw/q8Y2a836"))()
                end
            })

            -- Fish Game Section
            local Tab = Window:MakeTab({
                Name = "Fish Game",
                Icon = "rbxassetid://4483345998",
                PremiumOnly = false
            })
            Tab:AddButton({
                Name = "SpeedHub {OP}",
                Callback = function()
                    loadstring(game:HttpGet("https://raw.githubusercontent.com/AhmadV99/Speed-Hub-X/main/Speed%20Hub%20X.lua", true))()
                end    
            })

            -- Funky Friday Section
            local Tab = Window:MakeTab({
                Name = "Funky Friday",
                Icon = "rbxassetid://4483345998",
                PremiumOnly = false
            })
            Tab:AddButton({
                Name = "Funky Friday Hub {OP}",
                Callback = function()
                    loadstring(game:HttpGet('https://pastebin.com/raw/dcyuEgyK'))()
                end
            })

            -- Rivals Section
            local Tab = Window:MakeTab({
                Name = "Rivals",
                Icon = "rbxassetid://4483345998",
                PremiumOnly = false
            })
            Tab:AddButton({
                Name = "Neutron Hub {OP}",
                Callback = function()
                    loadstring(game:HttpGet("https://raw.githubusercontent.com/PawsThePaw/Neutron.lua/refs/heads/main/V1.0.2.txt", true))()
                end
            })

            -- AUT Section
            local Tab = Window:MakeTab({
                Name = "AUT",
                Icon = "rbxassetid://4483345998",
                PremiumOnly = false
            })
            Tab:AddButton({
                Name = "Demonic Hub {NEW}",
                Callback = function()
                    loadstring(game:HttpGet("https://raw.githubusercontent.com/OhhMyGehlee/Mul/refs/heads/main/ver"))()
                end
            })

            -- Sol's RNG Section
            local Tab = Window:MakeTab({
                Name = "Sols RNG",
                Icon = "rbxassetid://4483345998",
                PremiumOnly = false
            })
            Tab:AddButton({
                Name = "Erudite Hub {NEW}",
                Callback = function()
                    loadstring(game:HttpGet("https://raw.githubusercontent.com/ThacG/EruditeHub/main/Sol's%20RNG/V2.69"))()
                end
            })

            -- Vehicle Legends Section
            local Tab = Window:MakeTab({
                Name = "Vehicle Legends",
                Icon = "rbxassetid://4483345998",
                PremiumOnly = false
            })
            Tab:AddButton({
                Name = "Vesta Hub {NEW}",
                Callback = function()
                    loadstring(game:HttpGet("https://raw.githubusercontent.com/Marco8642/science/main/Vehicle%20legends"))()
                end
            })

            OrionLib:Init()
        else
            OrionLib:MakeNotification({
                Name = "❌ Incorrect",
                Content = "Key Incorrect! Try again.",
                Image = "rbxassetid://4483345998",
                Time = 3
            })
        end
    end
})

-- Get Key Button
KeyTab:AddButton({
    Name = "Get Key",
    Callback = function()
        setclipboard(KeyLink)
        OrionLib:MakeNotification({
            Name = "🔗 Link Copied",
            Content = "Key link has been copied to your clipboard!",
            Image = "rbxassetid://4483345998",
            Time = 3
        })
    end
})

OrionLib:Init()