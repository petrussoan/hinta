	-- Gui to Lua
	-- Version: 3.2

	-- Instances:

	local ScreenGui = Instance.new("ScreenGui")
	local Mys = Instance.new("Frame")
	local UICorner = Instance.new("UICorner")
	local GetOutfit = Instance.new("TextButton")
	local UICorner_2 = Instance.new("UICorner")
	local TextLabel = Instance.new("TextLabel")
	local UICorner_3 = Instance.new("UICorner")
	local Byakugan = Instance.new("TextButton")
	local UICorner_4 = Instance.new("UICorner")
	local _2 = Instance.new("TextButton")
	local UICorner_5 = Instance.new("UICorner")

	--Properties:

	ScreenGui.Parent = game.CoreGui
	ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

	Mys.Name = "Mys"
	Mys.Parent = ScreenGui
	Mys.BackgroundColor3 = Color3.fromRGB(91, 91, 91)
	Mys.Position = UDim2.new(0.388092637, 0, 0.192066804, 0)
	Mys.Size = UDim2.new(0, 323, 0, 282)
	Mys.Draggable = true
	Mys.Active = true

	UICorner.Parent = Mys

	GetOutfit.Name = "Get Outfit"
	GetOutfit.Parent = Mys
	GetOutfit.BackgroundColor3 = Color3.fromRGB(70, 70, 70)
	GetOutfit.BorderSizePixel = 0
	GetOutfit.Position = UDim2.new(0.211009175, 0, 0.27509293, 0)
	GetOutfit.Size = UDim2.new(0, 200, 0, 50)
	GetOutfit.Font = Enum.Font.SourceSansBold
	GetOutfit.Text = "Get Outfit"
	GetOutfit.TextColor3 = Color3.fromRGB(255, 255, 255)
	GetOutfit.TextSize = 20.000

	UICorner_2.Parent = GetOutfit

	TextLabel.Parent = Mys
	TextLabel.BackgroundColor3 = Color3.fromRGB(102, 102, 102)
	TextLabel.BorderSizePixel = 0
	TextLabel.Position = UDim2.new(0.211009175, 0, 0, 0)
	TextLabel.Size = UDim2.new(0, 213, 0, 50)
	TextLabel.Font = Enum.Font.SourceSans
	TextLabel.Text = "Hinata Byakugan"
	TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
	TextLabel.TextSize = 23.000

	UICorner_3.Parent = TextLabel

	Byakugan.Name = "Byakugan!"
	Byakugan.Parent = Mys
	Byakugan.BackgroundColor3 = Color3.fromRGB(70, 70, 70)
	Byakugan.BorderSizePixel = 0
	Byakugan.Position = UDim2.new(0.192660555, 0, 0.617100358, 0)
	Byakugan.Size = UDim2.new(0, 124, 0, 47)
	Byakugan.Font = Enum.Font.SourceSansBold
	Byakugan.Text = "Byakugan! >"
	Byakugan.TextColor3 = Color3.fromRGB(255, 255, 255)
	Byakugan.TextSize = 20.000

	UICorner_4.Parent = Byakugan

	_2.Name = "2"
	_2.Parent = Mys
	_2.BackgroundColor3 = Color3.fromRGB(131, 130, 132)
	_2.BorderSizePixel = 0
	_2.Position = UDim2.new(0.636085629, 0, 0.635687709, 0)
	_2.Size = UDim2.new(0, 68, 0, 36)
	_2.Font = Enum.Font.SourceSansBold
	_2.Text = ""
	_2.TextColor3 = Color3.fromRGB(253, 251, 255)
	_2.TextSize = 20.000

	UICorner_5.Parent = _2

	-- Scripts:

	local function TKUL_fake_script() -- GetOutfit.LocalScript 
		local script = Instance.new('LocalScript', GetOutfit)

		script.Parent.MouseButton1Click:Connect(function()

			local Animate = game.Players.LocalPlayer.Character.Animate

			--local idleAnim = char.Humanoid:LoadAnimation(char.Humanoid.Fly)
			--local forwardAnim = char.Humanoid:LoadAnimation(char.Humanoid.Hover)


			--PLAY
			--char.Animate.Disabled = true
			--idleAnim:Play()



			--STOP

			--char.Animate.Disabled = false
			--idleAnim:Stop()
			--forwardAnim:Stop()
			game.Players.LocalPlayer.Character.Pants.PantsTemplate = "rbxassetid://6525422082"
			game.Players.LocalPlayer.Character.Shirt.ShirtTemplate ="rbxassetid://6525421388"
			game.Players.LocalPlayer.Character.Head.face.Texture="rbxassetid://7109812423"

			Animate.idle.Animation1.AnimationId = "http://www.roblox.com/asset/?id=782841498"
			Animate.idle.Animation2.AnimationId = "http://www.roblox.com/asset/?id=782845736"
			Animate.walk.WalkAnim.AnimationId = "http://www.roblox.com/asset/?id=656121766"
			Animate.run.RunAnim.AnimationId = "http://www.roblox.com/asset/?id=656118852"
			Animate.jump.JumpAnim.AnimationId = "http://www.roblox.com/asset/?id=656117878"
			Animate.climb.ClimbAnim.AnimationId = "http://www.roblox.com/asset/?id=656114359"
			Animate.fall.FallAnim.AnimationId = "http://www.roblox.com/asset/?id=656115606"
			game.Players.LocalPlayer.Character.Humanoid.Jump = true

			local notifSound = Instance.new("Sound",workspace)

			local notifSound = Instance.new("Sound",workspace)
			notifSound.PlaybackSpeed = 1
			notifSound.Volume = 16
			notifSound.SoundId = "rbxassetid://5258216212"
			notifSound.PlayOnRemove = true
			notifSound:Destroy()


		end)
	end
	coroutine.wrap(TKUL_fake_script)()
	local function PBHOHS_fake_script() -- Byakugan.LocalScript 
		local script = Instance.new('LocalScript', Byakugan)

		script.Parent.MouseButton1Click:Connect(function()


			local notifSound = Instance.new("Sound",workspace)

			local notifSound = Instance.new("Sound",workspace)
			notifSound.PlaybackSpeed = 1
			notifSound.Volume = 16
			notifSound.SoundId = "rbxassetid://7551332288"
			notifSound.PlayOnRemove = true
			notifSound:Destroy()


			wait(0.30)



			chams = true
			repeat wait(0)
				function CreateSG(name,parent,face)
					local SurfaceGui = Instance.new("SurfaceGui",parent)
					SurfaceGui.Parent = parent
					SurfaceGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
					SurfaceGui.Face = Enum.NormalId[face]
					SurfaceGui.LightInfluence = 0
					SurfaceGui.ResetOnSpawn = false
					SurfaceGui.Name = name
					SurfaceGui.AlwaysOnTop = true
					local Frame = Instance.new("Frame",SurfaceGui)
					Frame.BackgroundColor3 = Color3.fromRGB(103, 102, 104)
					Frame.Size = UDim2.new(1,0,1,0)
				end

				while wait(1) do
					for i,v in pairs (game:GetService("Players"):GetPlayers()) do
						if v ~= game:GetService("Players").LocalPlayer and v.Character ~= nil and v.Character:FindFirstChild("Head") and v.Character.Head:FindFirstChild("cham") == nil then
							for i,v in pairs (v.Character:GetChildren()) do
								if v:IsA("MeshPart") or v.Name == "Head" then
									CreateSG("cham",v,"Back")
									CreateSG("cham",v,"Front")
									CreateSG("cham",v,"Left")
									CreateSG("cham",v,"Right")
									CreateSG("cham",v,"Right")
									CreateSG("cham",v,"Top")
									CreateSG("cham",v,"Bottom")
								end
							end
						end
					end
				end
			until chams == false
		end)
	end
	coroutine.wrap(PBHOHS_fake_script)()
