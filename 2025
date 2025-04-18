local Rayfield = loadstring(game:HttpGet('https://sirius.menu/rayfield'))()

local Window = Rayfield:CreateWindow({
   Name = "Raposinho Hub / Scripts 2.0 ",
   Icon = 0, -- Icon in Topbar. Can use Lucide Icons (string) or Roblox Image (number). 0 to use no icon (default).
   LoadingTitle = "Bem vindo a Raposa HUB 👑",
   LoadingSubtitle = "utilizando versão computador",
   Theme = "black light",

   DisableRayfieldPrompts = true,
   DisableBuildWarnings = false, -- Prevents Rayfield from warning when the script has a version mismatch with the interface

   ConfigurationSaving = {
      Enabled = true,
      FolderName = nil, -- Create a custom folder for your hub/game
      FileName = "Raposa Hub"
   },

   Discord = {
      Enabled = false, -- Prompt the user to join your Discord server if their executor supports it
      Invite = "noinvitelink", -- The Discord invite code, do not include discord.gg/. E.g. discord.gg/ ABCD would be ABCD
      RememberJoins = true -- Set this to false to make them join the discord every time they load it up
   },

   KeySystem = true, -- Set this to true to use our key system
   KeySettings = {
      Title = " 🔐 Acesso Bloqueado - Computador",
      Subtitle = "usuarios de pc contém a chave",
      Note = "Esta versão é desbloqueada apenas para computadores", -- Use this to tell the user how to get a key
      FileName = "Key", -- It is recommended to use something unique as other scripts using Rayfield may overwrite your key file
      SaveKey = false, -- The user's key will be saved, but if you change the key, they will be unable to use your script
      GrabKeyFromSite = false, -- If this is true, set Key below to the RAW site you would like Rayfield to get the key from
      Key = {"sucesso"} -- List of keys that will be accepted by the system, can be RAW file links (pastebin, github etc) or simple strings ("hello","key22")
   }
})

local Tab = Window:CreateTab("Jogador", 72186283700524)

local Section = Tab:CreateSection("Section Example")

Section:Set("Section Example")

local Divider = Tab:CreateDivider()

Divider:Set(false) -- Whether the divider's visibility is to be set to true or false.

Rayfield:Notify({
   Title = "Obrigado",
   Content = "Desenvolvedor: Bio_xy7890 🇧🇷",
   Duration = 10,
   Image = 76089771937509,
})

local Button = Tab:CreateButton({
   Name = "Button Example",
   Callback = function()
   local plr = game.Players.LocalPlayer

function resetPlr()
    if plr.Character then
        plr.Character:BreakJoints()
    end
end

resetPlr()

   game:GetService("ReplicatedStorage")["Remotes"]["Reset"]:FireServer()
   -- The function that takes place when the button is pressed
   end,
})

local Toggle = Tab:CreateToggle({
   Name = "Auto Clicker",
   CurrentValue = false,
   Flag = "Toggle1", -- A flag is the identifier for the configuration file, make sure every element has a different flag if you're using configuration saving to ensure no overlaps
   Callback = function(Value)
   player.Character.Humanoid.Walkspeed = 200
   end 
   })

local Slider = Tab:CreateSlider({
   Name = "Velocidade",
   Range = {15, 200},
   Increment = 15,
   Suffix = "de velocidade",
   CurrentValue = 10,
   Flag = "Velocidade", -- A flag is the identifier for the configuration file, make sure every element has a different flag if you're using configuration saving to ensure no overlaps
   Callback = function(Value)
   -- The function that takes place when the slider changes
   -- The variable (Value) is a number which correlates to the value the slider is currently at
   end,
})
