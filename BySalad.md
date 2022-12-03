if game:GetService("CoreGui"):FindFirstChild("Auto Event") then
   game:GetService("CoreGui"):FindFirstChild("Auto Event"):Destroy()
end
local UILib = loadstring(game:HttpGet('https://raw.githubusercontent.com/kickTh/New-Ui/main/ABC_Ui.txt'))()

local win = UILib:Window("Salad Auto Event",Color3.fromRGB(44, 120, 224), Enum.KeyCode.RightControl)
local MainSection = win:Tab("Main")

MainSection:Button("Auto Chest", function()loadstring(game:HttpGet("https://raw.githubusercontent.com/scriptpastebin/raw/main/ChestFarm"))()

end)

MainSection:Toggle("Toggle",false, function()_G.AutoConfetti = true -- Dont delete this
loadstring(game:HttpGet("https://pastebin.com/raw/K8jMXmQJ"))()

end)

local Settings = win:Tab("Settings")
Settings:Label("UI Toggle Key:  Right-Ctrl")
Settings:Label("Credit : Salad")
Settings:Button("Copy Discord Invite", function()
    setclipboard("https://discord.gg/hMkMXA5bRV")
    UILib:Notification("Notification", "Copied!", "Okay")
end)
Settings:Button("FreeBobux", function()
   setclipboard("you are stupid")
   UILib:Notification("Notification", "Copied!", "Okay")
end)
