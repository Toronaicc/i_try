game.Players.PlayerAdded:Connect(function(plr)
local ls = Instance.new("Folder",plr)
ls.Name = "leaderstats"
local clicks = Instance.new("IntValue",ls)
clicks.Name = "Taps"
clicks.Value = 0
end)
