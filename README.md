if game.CoreGui:FindFirstChild("Blackout") then
    game.CoreGui:FindFirstChild("Blackout"):Destroy()
end

local blackScreen = Instance.new("ScreenGui")
blackScreen.Name = "Blackout"
blackScreen.IgnoreGuiInset = true
blackScreen.ResetOnSpawn = false

local frame = Instance.new("Frame")
frame.Size = UDim2.new(1, 0, 1, 0)
frame.Position = UDim2.new(0, 0, 0, 0)
frame.BackgroundColor3 = Color3.new(0, 0, 0)
frame.BorderSizePixel = 0
frame.Parent = blackScreen

blackScreen.Parent = game:GetService("CoreGui")
