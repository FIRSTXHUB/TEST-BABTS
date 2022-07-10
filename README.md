local SimpleUi = loadstring(game:HttpGet("https://raw.githubusercontent.com/naypramx/Ui__Project/Script/Asss"))()
local Ui = SimpleUi:Win('FRIST X')
local Chanel = Ui:Channel('FRIST MENU')

local Page = Chanel:Addpage('Auto Farm')

Page:Button("Button!",function()
     game.Players.localPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-53.5656891, 50.9999924, -345.506866, 1, 0, 0, 0, 1, 0, 0, 0, 1)
	 wait(0.5)
local TweenService = game:GetService("TweenService")

local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(25, Enum.EasingStyle.Linear, Enum.EasingDirection.In,0,false,0),
{CFrame = CFrame.new(-52.7291145, 96.3343353, 8746.8584, -0.998737693, -0.00385044701, 0.0500821695, 1.24760269e-09, 0.997057557, 0.0766564012, -0.0502299666, 0.076559633, -0.995798945)}):Play()	
wait(25)
local TweenService = game:GetService("TweenService")

local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart, TweenInfo.new(5, Enum.EasingStyle.Linear, Enum.EasingDirection.In,0,false,0),
{CFrame = CFrame.new(-53.4292603, -359.10199, 9490.39844, -0.646022499, -1.17773613e-08, 0.76331836, -4.67346073e-09, 1, 1.14738503e-08, -0.76331836, 3.84502696e-09, -0.646022499)}):Play()
wait(0)
workspace.ClaimRiverResultsGold:FireServer()
end)
Page:Toggle("GOD_Mode_InWater!",false,function(t)
    game.Players.LocalPlayer.Character.WaterDetector:Destroy()
end)
Page:Toggle("Delete_Water!",false,function(t)
    game.Workspace.Water:Destroy()
end)
Page:slider("Slider!",1,100,16,function(h)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = h
end)
end)
Page:Label('Label!')
Page:line() 
