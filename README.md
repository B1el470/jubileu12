local radio = script.Parent

radio.Touched:Connect(function(hit players)
    local character = hit.Parent
    local humanoid = character:FindFirstChild("Humanoid")
    if humanoid then
        humanoid.Health = 0
    end
end)


