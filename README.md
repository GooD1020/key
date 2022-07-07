local Hwid = {

    [""] = "";

    [""] = "";

    [""] = "";

    [""] = ""

}

local ClientId = game:GetService("RbxAnalyticsService"):GetClientId()

local Hwide = string.split((ClientId), '-')

local Key = Hwide[1]



setclipboard("Key :".. (Key).." to> "..(ClientId))



if _G.Key == Key then

if Hwid[_G.Key] == game:GetService("RbxAnalyticsService"):GetClientId() then

if string.lower(game:GetService("RbxAnalyticsService"):GetClientId()) == game:GetService("RbxAnalyticsService"):GetClientId() then

    local ScreenGui = Instance.new("ScreenGui")

    local ImageButton = Instance.new("ImageButton")



    ScreenGui.Parent = game:GetService("Players").LocalPlayer:WaitForChild("PlayerGui")



    ImageButton.Parent = ScreenGui

    ImageButton.BackgroundColor3 = Color3.fromRGB(15, 15, 15)

    ImageButton.Position = UDim2.new(0.120833337, 0, 0.0952890813, 0)

    ImageButton.Size = UDim2.new(0, 50, 0, 50)

    ImageButton.Image = "rbxassetid://"

    ImageButton.MouseButton1Down:connect(function()

        game:GetService("VirtualInputManager"):SendKeyEvent(true,305,false,game)

        game:GetService("VirtualInputManager"):SendKeyEvent(false,305,false,game)

    end)

end
