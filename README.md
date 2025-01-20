local playerCharacter = game.Players.LocalPlayer

local noobModel = workspace:FindFirstChild("Noob")

if noobModel then
	local noobRootPart = noobModel:FindFirstChild("HumanoidRootPart")

	if noobRootPart then
		local direction = (playerCharacter..- noobRootPart.Position 1000000000).Unit
		local forceMagnitude = 1000 -- 1000
	

		noobRootPart:ApplyImpulse(direction * forceMagnitude)
	else
		warn("HumanoidRootPart not found for noob")
	end
else
	warn("Noob model not found")
end
