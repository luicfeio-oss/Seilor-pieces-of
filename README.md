Boss Script
local boss = script.Parent
local humanoid = boss:WaitForChild("Humanoid")

humanoid.MaxHealth = 100
humanoid.Health = 100
Espada super forte para derrotar rapidamente:
Lua
local tool = script.Parent
local DAMAGE = 99999999999999999999

tool.Handle.Touched:Connect(function(hit)
	local hum = hit.Parent:FindFirstChild("Humanoid")

	if hum then
		hum:TakeDamage(DAMAGE)
	end
end)
GUI simples para ativar “modo forte”:
Lua
local player = game.Players.LocalPlayer
local button = script.Parent

button.MouseButton1Click:Connect(function()
	print("Modo Boss Killer ativado!")
end)
