local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("Tayza X Hub", "Midnight")

-- Creadit
local Tab = Window:NewTab("Creadit")
local Section = Tab:NewSection("Creadit By")
Section:NewTextBox("Xx__tayza3333__xX")
local Section = Tab:NewSection("My roblox acc")
Section:NewTextBox("tayza3333")
Section:NewKeybind("z", "KeybindInfo", Enum.KeyCode.Z, function()
	Library:ToggleUI()
end)

local Tab = Window:NewTab("Main")
local Section = Tab:NewSection("Prestige farm")
Section:NewToggle("On-Off", "-", function(state)
    if state then
        local auto_farm = true
if auto_farm then
_G.toogle = true
local Plr = game:GetService("Players").LocalPlayer
function tp(plr, endpos)
    plr.character.HumanoidRootPart.CFrame = CFrame.new(endpos)
end
local Pos = Vector3.new(-495, 148, 381)
    while _G.toogle do
        tp(Plr, Pos)
        wait(0.01)
    end
else
if not auto_farm then
_G.toogle = false
    game_()
end
end
    else
        local auto_farm = false
if auto_farm then
_G.toogle = true
local Plr = game:GetService("Players").LocalPlayer
function tp(plr, endpos)
    plr.character.HumanoidRootPart.CFrame = CFrame.new(endpos)
end
local Pos = Vector3.new(-495, 148, 381)
    while _G.toogle do
        tp(Plr, Pos)
        wait(0.01)
    end
else
if not auto_farm then
_G.toogle = false
    game_()
end
end
    end
end)
local Section = Tab:NewSection("Checkpoints farm")
Section:NewButton("Open", "-", function()
    local start_stage = 1 --stage you want to start
local end_stage = 550 --stage you want to end
local wait_time = 0.1 --longer wait time will reduce missing chance
local todo = game:GetService("Workspace").Stages:GetChildren()
local Plr = game:GetService("Players").LocalPlayer

function tp(plr, endpos)
    plr.character.HumanoidRootPart.CFrame = CFrame.new(endpos)
end

for j = start_stage, end_stage, 1 do
for i,v in pairs(todo) do
        if todo[i].name == tostring(j) then
            local todo_2 = todo[i]:GetChildren()
            for t,v in pairs(todo_2) do
                if todo_2[t].name == "Spawn" then
                    local Pos = todo_2[t].Position
                    tp(Plr, Pos)
                    wait(wait_time)
                    break
                end
            end
        end
    end
end
end)
