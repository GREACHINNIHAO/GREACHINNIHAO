-- SCRIPTWARE OFFICAL HUB
local lib = loadstring(game:HttpGet("https://raw.githubusercontent.com/AZYsGithub/Arceus-X-UI-Library/main/source.lua"))()
lib:SetTitle("Arceus X Gravity")
lib:SetIcon("http://www.roblox.com/asset/?id=9178187770")
local a = workspace.Gravity

lib:SetTheme("Default")
lib:AddButton("Reset", function()
    game.Players.LocalPlayer.Character.Head:Destroy()
end)

lib:AddToggle("Toggle Moon Gravity", function(state)
    if state then
        workspace.Gravity = 60
    else
        workspace.Gravity = a
    end
end, false)
