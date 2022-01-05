local player = game.Players.LocalPlayer
local spamtalklevel = {"whos gvvy?", "LGBTQ sucks!", "gvvy people", "XLMAO", "lol, funny", "what do yall think of LGBTQ", "i don't support."}
local mouse = player:GetMouse()

function talk(key)
key = key:lower()
if key == "t" then
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(spamtalklevel[math.random(1,#spamtalklevel)], "All")
end
end
mouse.KeyDown:Connect(talk)
