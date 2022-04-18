-- Gui to Lua
-- Version: 3.2

-- Instances:

local LoadGui = Instance.new("ScreenGui")
local Background = Instance.new("ImageLabel")
local UICorner = Instance.new("UICorner")
local Creator = Instance.new("TextLabel")
local LoadingProgress = Instance.new("ImageLabel")
local OutPot = Instance.new("TextLabel")
local Build = Instance.new("TextLabel")
local OnScript = Instance.new("TextButton")
local UICorner_2 = Instance.new("UICorner")
local OFFScript = Instance.new("TextButton")
local UICorner_3 = Instance.new("UICorner")
local Hwid = Instance.new("TextLabel")
local UICorner_4 = Instance.new("UICorner")

--Properties:

LoadGui.Name = "Load Gui"
LoadGui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
LoadGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

Background.Name = "Background"
Background.Parent = LoadGui
Background.Active = true
Background.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Background.BackgroundTransparency = 1.000
Background.BorderSizePixel = 0
Background.Position = UDim2.new(0.407255888, 0, 0.228621811, 0)
Background.Size = UDim2.new(0, 319, 0, 278)
Background.Image = "rbxasset://textures/loading/LoadingTexture.png"
Background.ImageColor3 = Color3.fromRGB(50, 50, 50)
Background.SliceCenter = Rect.new(0, 0, 350, 350)

UICorner.CornerRadius = UDim.new(0, 15)
UICorner.Parent = Background

Creator.Name = "Creator"
Creator.Parent = Background
Creator.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Creator.BackgroundTransparency = 1.000
Creator.Position = UDim2.new(-0.0017374903, 0, 0.879813135, 0)
Creator.Size = UDim2.new(0, 164, 0, 26)
Creator.Font = Enum.Font.Arial
Creator.Text = "By: WTF Hub"
Creator.TextColor3 = Color3.fromRGB(179, 229, 255)
Creator.TextSize = 20.000
Creator.TextWrapped = true

LoadingProgress.Name = "LoadingProgress"
LoadingProgress.Parent = Background
LoadingProgress.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
LoadingProgress.BackgroundTransparency = 1.000
LoadingProgress.BorderSizePixel = 0
LoadingProgress.Position = UDim2.new(0.66931361, 0, 0.622158647, 0)
LoadingProgress.Size = UDim2.new(0, 105, 0, 105)
LoadingProgress.Image = "rbxassetid://1078907462"

OutPot.Name = "Out Pot"
OutPot.Parent = Background
OutPot.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
OutPot.BackgroundTransparency = 1.000
OutPot.Position = UDim2.new(-0.0236810669, 0, 0.0717990771, 0)
OutPot.Size = UDim2.new(0, 257, 0, 34)
OutPot.Font = Enum.Font.Arial
OutPot.Text = "LoadScript"
OutPot.TextColor3 = Color3.fromRGB(255, 193, 130)
OutPot.TextScaled = true
OutPot.TextSize = 14.000
OutPot.TextWrapped = true

Build.Name = "Build"
Build.Parent = Background
Build.BackgroundColor3 = Color3.fromRGB(255, 0, 0)
Build.BackgroundTransparency = 1.000
Build.Position = UDim2.new(0.208293855, 0, 0.232331097, 0)
Build.Size = UDim2.new(0, 236, 0, 26)
Build.Font = Enum.Font.Arial
Build.Text = "Build A Boat For Treasure"
Build.TextColor3 = Color3.fromRGB(255, 178, 179)
Build.TextSize = 20.000
Build.TextWrapped = true

OnScript.Name = "On Script"
OnScript.Parent = Background
OnScript.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
OnScript.BackgroundTransparency = 1.000
OnScript.Position = UDim2.new(0.0908645689, 0, 0.185714051, 0)
OnScript.Size = UDim2.new(0, 55, 0, 28)
OnScript.Visible = false
OnScript.Font = Enum.Font.SourceSans
OnScript.Text = "On Script"
OnScript.TextColor3 = Color3.fromRGB(6, 255, 26)
OnScript.TextSize = 14.000

UICorner_2.Parent = OnScript

OFFScript.Name = "OFF Script"
OFFScript.Parent = OnScript
OFFScript.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
OFFScript.BackgroundTransparency = 1.000
OFFScript.Position = UDim2.new(3.92722821, 0, -0.0285716653, 0)
OFFScript.Size = UDim2.new(0, 55, 0, 28)
OFFScript.Font = Enum.Font.SourceSans
OFFScript.Text = "OFF Script"
OFFScript.TextColor3 = Color3.fromRGB(255, 0, 0)
OFFScript.TextSize = 14.000

UICorner_3.Parent = OFFScript

Hwid.Name = "Hwid"
Hwid.Parent = Background
Hwid.BackgroundColor3 = Color3.fromRGB(76, 76, 76)
Hwid.Position = UDim2.new(0.057, 0, 0.108999997, 0)
Hwid.Size = UDim2.new(0, 1, 0, 36)
Hwid.Visible = false
Hwid.Font = Enum.Font.SourceSans
Hwid.Text = ""
Hwid.TextColor3 = Color3.fromRGB(255, 255, 255)
Hwid.TextSize = 14.000

UICorner_4.Parent = Hwid

-- Scripts:

local function ATNC_fake_script() -- Creator.Transparency 
	local script = Instance.new('Script', Creator)

	
	wait(5)
	script.Parent.TextTransparency = 0.1
	wait(0.1)
	script.Parent.TextTransparency = 0.2
	wait(0.1)
	script.Parent.TextTransparency = 0.3
	wait(0.1)
	script.Parent.TextTransparency = 0.4
	wait(0.1)
	script.Parent.TextTransparency = 0.5
	wait(0.1)
	script.Parent.TextTransparency = 0.6
	wait(0.1)
	script.Parent.TextTransparency = 0.7
	wait(0.1)
	script.Parent.TextTransparency = 0.8
	wait(0.1)
	script.Parent.TextTransparency = 0.9
	wait(0.1)
	script.Parent.TextTransparency = 1
	-- for some reason the transparency for this wont work in the main script.
end
coroutine.wrap(ATNC_fake_script)()
local function HJIFNOT_fake_script() -- LoadingProgress.Script 
	local script = Instance.new('Script', LoadingProgress)

	while wait(.01) do
	script.Parent.Rotation = script.Parent.Rotation + 5
	end
end
coroutine.wrap(HJIFNOT_fake_script)()
local function ZKNHSP_fake_script() -- LoadingProgress.Transparency 
	local script = Instance.new('Script', LoadingProgress)

	wait(5.5)
	script.Parent.Visible = false
	wait(0.5)
	script.Parent.Parent.Parent.Background:TweenSize(UDim2.new(0, 331,0, 46))
	wait(1)
	script.Parent.Parent["On Script"].Visible = true
end
coroutine.wrap(ZKNHSP_fake_script)()
local function DOBPNY_fake_script() -- OutPot.Transparency 
	local script = Instance.new('Script', OutPot)

	
	wait(5)
		script.Parent.TextTransparency = 0.1
		wait(0.1)
		script.Parent.TextTransparency = 0.2
		wait(0.1)
		script.Parent.TextTransparency = 0.3
		wait(0.1)
		script.Parent.TextTransparency = 0.4
		wait(0.1)
		script.Parent.TextTransparency = 0.5
		wait(0.1)
		script.Parent.TextTransparency = 0.6
		wait(0.1)
		script.Parent.TextTransparency = 0.7
		wait(0.1)
		script.Parent.TextTransparency = 0.8
		wait(0.1)
		script.Parent.TextTransparency = 0.9
		wait(0.1)
		script.Parent.TextTransparency = 1
	-- for some reason the transparency for this wont work in the main script.
end
coroutine.wrap(DOBPNY_fake_script)()
local function FFOX_fake_script() -- Build.Transparency 
	local script = Instance.new('Script', Build)

	
	wait(5)
	script.Parent.TextTransparency = 0.1
	wait(0.1)
	script.Parent.TextTransparency = 0.2
	wait(0.1)
	script.Parent.TextTransparency = 0.3
	wait(0.1)
	script.Parent.TextTransparency = 0.4
	wait(0.1)
	script.Parent.TextTransparency = 0.5
	wait(0.1)
	script.Parent.TextTransparency = 0.6
	wait(0.1)
	script.Parent.TextTransparency = 0.7
	wait(0.1)
	script.Parent.TextTransparency = 0.8
	wait(0.1)
	script.Parent.TextTransparency = 0.9
	wait(0.1)
	script.Parent.TextTransparency = 1
	-- for some reason the transparency for this wont work in the main script.
end
coroutine.wrap(FFOX_fake_script)()
local function CVDOOV_fake_script() -- Background.LocalScript 
	local script = Instance.new('LocalScript', Background)

	
	frame = script.Parent.Parent.Background
	frame.Draggable = true
	frame.Selectable = true
	frame.Active = true
end
coroutine.wrap(CVDOOV_fake_script)()
local function VOWFFRE_fake_script() -- OFFScript.LocalScript 
	local script = Instance.new('LocalScript', OFFScript)

	script.Parent.MouseButton1Click:Connect(function ()
		script.Parent.Parent.Parent.Parent.Background:Destroy()
	end)
end
coroutine.wrap(VOWFFRE_fake_script)()
local function ZHTYZON_fake_script() -- OnScript.LocalScript 
	local script = Instance.new('LocalScript', OnScript)

	
	script.Parent.MouseButton1Click:Connect(function ()
		script.Parent["OFF Script"].Visible = false
		script.Parent.Parent["On Script"].Visible = false
	    script.Parent.Parent.Hwid.Visible = true
		script.Parent.Parent.Hwid:TweenSize(UDim2.new(0, 295,0, 36))
		script.Parent.Parent.Hwid.Text = "_-Hwid-_"
		wait(1.5)
		local Hwid = loadstring(game:HttpGet"https://raw.githubusercontent.com/Minecarfh/Hwid/main/README.md")() 
		local HwidC = game:GetService("RbxAnalyticsService"):GetClientId()
		for i,v in pairs(Hwid) do 
			if v == HwidC then 
				script.Parent.Parent.Hwid.Text = ":-Hwid : Successful"
				wait(.5)
				script.Parent.Parent.Parent.Parent["Load Gui"]:Destroy()
				wait(.5)
				local gP = game.PlaceId

if gP == 537413528 then
	loadstring(game:HttpGet"https://best-wh-bi.000webhostapp.com/Build%20A%20Boat%20For%20Treasure")() 
elseif gP == 2753915549 or gP == 4442272183 or gP == 7449423635 or gP == 4520749081 or gP == 6381829480 then
	loadstring(game:HttpGet('https://androssy.net/files/Loader.lua')){43374,51548,35252,40090,23816,78627}
elseif gP == 8694898220 then
	local old
	local path = game.Players.LocalPlayer.Backpack
	old = hookmetamethod(path, "__index", function(instances,property)
		if tostring(instances) == "CurrentAmmo" and property == "Value" then
			return math.huge
		end
		return old(instances,property)
	end)
	loadstring(game:HttpGet"https://gist.githubusercontent.com/IYU23HR98HF/dc62e4ebfd0d1057cfc255cd35348bbd/raw/13dbaa2ab3261eb834a55048f1e4c90b6a2894a6/All%20Of%20Us%20Are%20Dead%20Script")()
end
			else 
				script.Parent.Parent.Hwid.Text = ":-Hwid : UnSuccessful"
				wait(2.5)
				script.Parent.Parent.Hwid.Text = "Rejoin"
				wait(.5)
				local tpservice= game:GetService("TeleportService")
				local plr = game.Players.LocalPlayer
	
				tpservice:Teleport(game.PlaceId, plr)
			end
		end
	end)
end
coroutine.wrap(ZHTYZON_fake_script)()
