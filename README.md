game.Players.PlayerAdded:Connect(function(plr)
local ls = Instance.new("Folder",plr)
ls.Name = "leaderstats"
local clicks = Instance.new("IntValue",ls)
clicks.Name = "Taps"
clicks.Value = 0
end)







local clicks = game.Players.LocalPlayer.leaderstats.Taps
local de = false
local T = 0.1
script.Parent.MouseButton1Click:Connect(function()
if de then
return
end
de = true
clicks.Value += 1
wait(T)
de = false
end)



local clicks = game.Players.LocalPlayer.leaderstats.Taps
while wait() do
script.Parent.Text = "Taps: " .. clicks.Value
end





script.Parent.MouseButton1Click:Connect(function()
    script.Parent.Parent.Frame.Visible = true
end)
