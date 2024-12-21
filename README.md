local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()

-- Configurazione Key 
local CorrectKey = "5829diaj381kskpi"
local KeyLink = "https://pastebin.com/xpNHZRzq" -- Sostituisci con un link reale
local ConfigFolder = "KeyVerification" -- Cartella per il salvataggio

-- Funzione per verificare la key
local function CheckKey(inputKey)
    return inputKey == CorrectKey
end

-- Funzione per salvare la Key
local function SaveKey(key)
    if not isfolder(ConfigFolder) then
        makefolder(ConfigFolder)
    end
    writefile(ConfigFolder .. "/SavedKey.txt", key)
end

-- Funzione per caricare la Key salvata
local function LoadKey()
    if isfile(ConfigFolder .. "/SavedKey.txt") then
        return readfile(ConfigFolder .. "/SavedKey.txt")
    else
        return nil
    end
end

-- Caricamento della Key salvata
local SavedKey = LoadKey()

-- Finestra di Verifica Key
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

-- Input Key
KeyTab:AddTextbox({
    Name = "Enter Key",
    Default = SavedKey or "", -- Mostra la Key salvata se disponibile
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
            -- Salva la Key corretta
            SaveKey(userKey)

            OrionLib:MakeNotification({
                Name = "✅ Verification Completed",
                Content = "Correct Key! Loading script...",
                Image = "rbxassetid://4483345998",
                Time = 3
            })

            wait(2)
            OrionLib:Destroy()

            -- Apri il sistema principale
            local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()
            local Window = OrionLib:MakeWindow({Name = "OrionLib | Hub", HidePremium = false, SaveConfig = true, ConfigFolder = "Orion"})

            -- Sezione Blox Fruits
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

            -- Sezione Universal
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

            -- Sezione Blade Ball
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

            -- Sezione Strongest Battlegrounds
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

            -- Sezione Fisch Game
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

            -- Sezione Funky Friday
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

            -- Sezione Rivals
            local Tab = Window:MakeTab({
                Name = "Rivals",
                Icon = "rbxassetid://4483345998",
                PremiumOnly = false
            })
            Tab:AddButton({
                Name = "Neutron Hub{OP}",
                Callback = function()
                    loadstring(game:HttpGet("https://raw.githubusercontent.com/PawsThePaw/Neutron.lua/refs/heads/main/V1.0.2.txt", true))()
                end
            })

            -- Sezione AUT
            local Tab = Window:MakeTab({
                Name = "Aut",
                Icon = "rbxassetid://4483345998",
                PremiumOnly = false
            })
            Tab:AddButton({
                Name = "Demonic Hub{NEW}",
                Callback = function()
                    loadstring(game:HttpGet("https://raw.githubusercontent.com/OhhMyGehlee/Mul/refs/heads/main/ver"))()
                end
            })

            -- Sezione Sol's RNG
            local Tab = Window:MakeTab({
                Name = "Sols rng",
                Icon = "rbxassetid://4483345998",
                PremiumOnly = false
            })
            Tab:AddButton({
                Name = "Erudite Hub{NEW}",
                Callback = function()
                    loadstring(game:HttpGet("https://raw.githubusercontent.com/ThacG/EruditeHub/main/Sol's%20RNG/V2.69"))()
                end
            })

            -- Sezione Vehicle Legends
            local Tab = Window:MakeTab({
                Name = "Vehicle Legends",
                Icon = "rbxassetid://4483345998",
                PremiumOnly = false
            })
            Tab:AddButton({
                Name = "Vesta Hub{NEW}",
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

-- Bottone per ottenere la Key
KeyTab:AddButton({
    Name = "Get Key",
    Callback = function()
        setclipboard(KeyLink)
        OrionLib:MakeNotification({
            Name = "🔗 Link Copiato",
            Content = "Link per ottenere la key è stato copiato negli appunti!",
            Image = "rbxassetid://4483345998",
            Time = 3
        })
    end
})

OrionLib:Init()
