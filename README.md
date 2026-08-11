local Players = game:GetService("Players")

local player = Players.LocalPlayer
local gui = Instance.new("ScreenGui")
gui.Name = "HelloDark"
gui.ResetOnSpawn = false
gui.Parent = player:WaitForChild("PlayerGui")

local box = Instance.new("Frame")
box.Size = UDim2.fromOffset(300, 150)
box.Position = UDim2.fromScale(0.5, 0.5)
box.AnchorPoint = Vector2.new(0.5, 0.5)
box.BackgroundColor3 = Color3.fromRGB(10, 25, 45)
box.BorderSizePixel = 0
box.Parent = gui

local corner = Instance.new("UICorner")
corner.CornerRadius = UDim.new(0, 12)
corner.Parent = box

local stroke = Instance.new("UIStroke")
stroke.Color = Color3.fromRGB(0, 140, 255)
stroke.Thickness = 2
stroke.Transparency = 0.15
stroke.Parent = box

local title = Instance.new("TextLabel")
title.Size = UDim2.new(1, -30, 0, 50)
title.Position = UDim2.fromOffset(15, 20)
title.BackgroundTransparency = 1
title.Text = "HELLO DARK"
title.TextColor3 = Color3.fromRGB(80, 180, 255)
title.TextSize = 28
title.Font = Enum.Font.GothamBold
title.Parent = box

local subtitle = Instance.new("TextLabel")
subtitle.Size = UDim2.new(1, -30, 0, 40)
subtitle.Position = UDim2.fromOffset(15, 75)
subtitle.BackgroundTransparency = 1
subtitle.Text = "Este é um pequeno teste."
subtitle.TextColor3 = Color3.fromRGB(200, 220, 240)
subtitle.TextSize = 16
subtitle.Font = Enum.Font.Gotham
subtitle.Parent = box
