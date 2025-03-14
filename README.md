			--WORKSPACE "MAP"
			local Map = Instance.new("Folder")
			Map.Name = "Map"
			Map.Parent = game:GetService("Workspace")

			local Ground = Instance.new("Part")
			Ground.Name = "Ground"
			Ground.TopSurface = Enum.SurfaceType.Smooth
			Ground.Color = Color3.new(0.12, 0.50, 0.11)
			Ground.Anchored = true
			Ground.Size = Vector3.new(250.00, 1.38, 260.76)
			Ground.BottomSurface = Enum.SurfaceType.Smooth
			Ground.BrickColor = BrickColor.new("Forest green")
			Ground.Position = Vector3.new(0.00, 9.69, -5.38)
			Ground.CFrame = CFrame.new(0.00, 9.69, -5.38, -0.00, -0.00, -1.00)
			Ground.Parent = Map

			local Top = Instance.new("Texture")
			Top.Name = "Top"
			Top.Face = Enum.NormalId.Top
			Top.StudsPerTileU = 9
			Top.Transparency = 0.9399999976158142
			Top.StudsPerTileV = 9
			Top.Texture = "http://www.roblox.com/asset/?id=6905014001"
			Top.Parent = Ground

			local Center = Instance.new("Part")
			Center.Name = "Center"
			Center.TopSurface = Enum.SurfaceType.Smooth
			Center.Color = Color3.new(0.55, 0.55, 0.55)
			Center.Anchored = true
			Center.Size = Vector3.new(25.00, 0.50, 25.00)
			Center.BottomSurface = Enum.SurfaceType.Smooth
			Center.BrickColor = BrickColor.new("Silver flip/flop")
			Center.Position = Vector3.new(0.00, 10.25, 0.00)
			Center.CFrame = CFrame.new(0.00, 10.25, 0.00, -0.00, -0.00, -1.00)
			Center.Parent = Map

			local Texture = Instance.new("Texture")
			Texture.Face = Enum.NormalId.Top
			Texture.StudsPerTileU = 9
			Texture.Transparency = 0.9599999785423279
			Texture.StudsPerTileV = 9
			Texture.Texture = "rbxassetid://6794119868"
			Texture.Parent = Center

			--WORKPLACE "PLOTS"
			local Plots = Instance.new("Folder")
			Plots.Name = "Plots"
			Plots.Parent = game:GetService("Workspace")

			local _ = Instance.new("Model")
			_.Name = "2"
			_.WorldPivot = CFrame.new(35.00, 10.58, -90.00, -0.00, -0.00, -1.00)
			_.Parent = Plots

			local Ground = Instance.new("Part")
			Ground.Name = "Ground"
			Ground.TopSurface = Enum.SurfaceType.Smooth
			Ground.Color = Color3.new(0.55, 0.55, 0.55)
			Ground.Anchored = true
			Ground.Size = Vector3.new(50.00, 0.50, 50.00)
			Ground.BottomSurface = Enum.SurfaceType.Smooth
			Ground.BrickColor = BrickColor.new("Silver flip/flop")
			Ground.Position = Vector3.new(35.00, 10.58, -90.00)
			Ground.CFrame = CFrame.new(35.00, 10.58, -90.00, -0.00, -0.00, -1.00)
			Ground.Parent = _

			local Texture = Instance.new("Texture")
			Texture.Face = Enum.NormalId.Top
			Texture.StudsPerTileU = 5
			Texture.Transparency = 0.9599999785423279
			Texture.StudsPerTileV = 5
			Texture.Texture = "rbxassetid://6794119868"
			Texture.Parent = Ground

			local Door = Instance.new("Model")
			Door.Name = "Door"
			Door.WorldPivot = CFrame.new(35.00, 14.33, -66.00, -0.00, -0.00, -1.00)
			Door.Parent = _

			local Door_1 = Instance.new("Part")
			Door_1.Name = "Door"
			Door_1.TopSurface = Enum.SurfaceType.Smooth
			Door_1.Color = Color3.new(0.21, 0.21, 0.21)
			Door_1.Anchored = true
			Door_1.Size = Vector3.new(6.00, 1.00, 1.00)
			Door_1.BottomSurface = Enum.SurfaceType.Smooth
			Door_1.BrickColor = BrickColor.new("Black")
			Door_1.Position = Vector3.new(35.00, 18.33, -65.50)
			Door_1.CFrame = CFrame.new(35.00, 18.33, -65.50, -0.00, -0.00, -1.00)
			Door_1.Parent = Door

			local Door_1 = Instance.new("Part")
			Door_1.Name = "Door"
			Door_1.TopSurface = Enum.SurfaceType.Smooth
			Door_1.Color = Color3.new(0.21, 0.21, 0.21)
			Door_1.Anchored = true
			Door_1.Size = Vector3.new(1.00, 8.00, 1.00)
			Door_1.BottomSurface = Enum.SurfaceType.Smooth
			Door_1.BrickColor = BrickColor.new("Black")
			Door_1.Position = Vector3.new(31.50, 14.83, -65.50)
			Door_1.CFrame = CFrame.new(31.50, 14.83, -65.50, -0.00, -0.00, -1.00)
			Door_1.Parent = Door

			local Door_1 = Instance.new("Part")
			Door_1.Name = "Door"
			Door_1.TopSurface = Enum.SurfaceType.Smooth
			Door_1.Color = Color3.new(0.21, 0.21, 0.21)
			Door_1.Anchored = true
			Door_1.Size = Vector3.new(1.00, 8.00, 1.00)
			Door_1.BottomSurface = Enum.SurfaceType.Smooth
			Door_1.BrickColor = BrickColor.new("Black")
			Door_1.Position = Vector3.new(38.50, 14.83, -65.50)
			Door_1.CFrame = CFrame.new(38.50, 14.83, -65.50, -0.00, -0.00, -1.00)
			Door_1.Parent = Door

			local Claim = Instance.new("Part")
			Claim.Name = "Claim"
			Claim.TopSurface = Enum.SurfaceType.Smooth
			Claim.Color = Color3.new(0.55, 0.55, 0.55)
			Claim.Anchored = true
			Claim.Size = Vector3.new(6.00, 7.00, 0.50)
			Claim.BottomSurface = Enum.SurfaceType.Smooth
			Claim.CanCollide = false
			Claim.Rotation = Vector3.new(180.00, 0.00, 180.00)
			Claim.Transparency = 0.25
			Claim.BrickColor = BrickColor.new("Silver flip/flop")
			Claim.Position = Vector3.new(35.00, 14.33, -65.50)
			Claim.CFrame = CFrame.new(35.00, 14.33, -65.50, 0.00, -0.00, 1.00)
			Claim.Parent = Door

			local SurfaceGui = Instance.new("SurfaceGui")
			SurfaceGui.LightInfluence = 1
			SurfaceGui.SizingMode = Enum.SurfaceGuiSizingMode.PixelsPerStud
			SurfaceGui.ClipsDescendants = true
			SurfaceGui.MaxDistance = 1000
			SurfaceGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
			SurfaceGui.Parent = Claim

			local TextLabel = Instance.new("TextLabel")
			TextLabel.TextWrapped = true
			TextLabel.BorderSizePixel = 0
			TextLabel.TextScaled = true
			TextLabel.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			TextLabel.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			TextLabel.TextSize = 14
			TextLabel.Size = UDim2.new(1.00, 0.00, 1.00, 0.00)
			TextLabel.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			TextLabel.Text = "Claim"
			TextLabel.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			TextLabel.BackgroundTransparency = 1
			TextLabel.Parent = SurfaceGui

			local UIStroke = Instance.new("UIStroke")
			UIStroke.Thickness = 4
			UIStroke.Parent = TextLabel

			local Claimed = Instance.new("StringValue")
			Claimed.Name = "Claimed"
			Claimed.Value = "None"
			Claimed.Parent = _

			local Upgrades = Instance.new("Folder")
			Upgrades.Name = "Upgrades"
			Upgrades.Parent = _

			local Buttons = Instance.new("Folder")
			Buttons.Name = "Buttons"
			Buttons.Parent = _

			local RobuxButtons = Instance.new("Folder")
			RobuxButtons.Name = "RobuxButtons"
			RobuxButtons.Parent = _

			local __1 = Instance.new("Model")
			__1.Name = "1"
			__1.WorldPivot = CFrame.new(-35.00, 10.58, -90.00, -0.00, -0.00, -1.00)
			__1.Parent = Plots

			local Ground_1 = Instance.new("Part")
			Ground_1.Name = "Ground"
			Ground_1.TopSurface = Enum.SurfaceType.Smooth
			Ground_1.Color = Color3.new(0.55, 0.55, 0.55)
			Ground_1.Anchored = true
			Ground_1.Size = Vector3.new(50.00, 0.50, 50.00)
			Ground_1.BottomSurface = Enum.SurfaceType.Smooth
			Ground_1.BrickColor = BrickColor.new("Silver flip/flop")
			Ground_1.Position = Vector3.new(-35.00, 10.58, -90.00)
			Ground_1.CFrame = CFrame.new(-35.00, 10.58, -90.00, -0.00, -0.00, -1.00)
			Ground_1.Parent = __1

			local Texture_1 = Instance.new("Texture")
			Texture_1.Face = Enum.NormalId.Top
			Texture_1.StudsPerTileU = 5
			Texture_1.Transparency = 0.9599999785423279
			Texture_1.StudsPerTileV = 5
			Texture_1.Texture = "rbxassetid://6794119868"
			Texture_1.Parent = Ground_1

			local Door_1 = Instance.new("Model")
			Door_1.Name = "Door"
			Door_1.WorldPivot = CFrame.new(-35.00, 14.33, -66.00, -0.00, -0.00, -1.00)
			Door_1.Parent = __1

			local Door_1 = Instance.new("Part")
			Door_1.Name = "Door"
			Door_1.TopSurface = Enum.SurfaceType.Smooth
			Door_1.Color = Color3.new(0.21, 0.21, 0.21)
			Door_1.Anchored = true
			Door_1.Size = Vector3.new(6.00, 1.00, 1.00)
			Door_1.BottomSurface = Enum.SurfaceType.Smooth
			Door_1.BrickColor = BrickColor.new("Black")
			Door_1.Position = Vector3.new(-35.00, 18.33, -65.50)
			Door_1.CFrame = CFrame.new(-35.00, 18.33, -65.50, -0.00, -0.00, -1.00)
			Door_1.Parent = Door_1

			local Door_1 = Instance.new("Part")
			Door_1.Name = "Door"
			Door_1.TopSurface = Enum.SurfaceType.Smooth
			Door_1.Color = Color3.new(0.21, 0.21, 0.21)
			Door_1.Anchored = true
			Door_1.Size = Vector3.new(1.00, 8.00, 1.00)
			Door_1.BottomSurface = Enum.SurfaceType.Smooth
			Door_1.BrickColor = BrickColor.new("Black")
			Door_1.Position = Vector3.new(-38.50, 14.83, -65.50)
			Door_1.CFrame = CFrame.new(-38.50, 14.83, -65.50, -0.00, -0.00, -1.00)
			Door_1.Parent = Door_1

			local Door_1 = Instance.new("Part")
			Door_1.Name = "Door"
			Door_1.TopSurface = Enum.SurfaceType.Smooth
			Door_1.Color = Color3.new(0.21, 0.21, 0.21)
			Door_1.Anchored = true
			Door_1.Size = Vector3.new(1.00, 8.00, 1.00)
			Door_1.BottomSurface = Enum.SurfaceType.Smooth
			Door_1.BrickColor = BrickColor.new("Black")
			Door_1.Position = Vector3.new(-31.50, 14.83, -65.50)
			Door_1.CFrame = CFrame.new(-31.50, 14.83, -65.50, -0.00, -0.00, -1.00)
			Door_1.Parent = Door_1

			local Claim_1 = Instance.new("Part")
			Claim_1.Name = "Claim"
			Claim_1.TopSurface = Enum.SurfaceType.Smooth
			Claim_1.Color = Color3.new(0.55, 0.55, 0.55)
			Claim_1.Anchored = true
			Claim_1.Size = Vector3.new(6.00, 7.00, 0.50)
			Claim_1.BottomSurface = Enum.SurfaceType.Smooth
			Claim_1.CanCollide = false
			Claim_1.Rotation = Vector3.new(180.00, 0.00, 180.00)
			Claim_1.Transparency = 0.25
			Claim_1.BrickColor = BrickColor.new("Silver flip/flop")
			Claim_1.Position = Vector3.new(-35.00, 14.33, -65.50)
			Claim_1.CFrame = CFrame.new(-35.00, 14.33, -65.50, 0.00, -0.00, 1.00)
			Claim_1.Parent = Door_1

			local SurfaceGui_1 = Instance.new("SurfaceGui")
			SurfaceGui_1.LightInfluence = 1
			SurfaceGui_1.SizingMode = Enum.SurfaceGuiSizingMode.PixelsPerStud
			SurfaceGui_1.ClipsDescendants = true
			SurfaceGui_1.MaxDistance = 1000
			SurfaceGui_1.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
			SurfaceGui_1.Parent = Claim_1

			local TextLabel_1 = Instance.new("TextLabel")
			TextLabel_1.TextWrapped = true
			TextLabel_1.BorderSizePixel = 0
			TextLabel_1.TextScaled = true
			TextLabel_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			TextLabel_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			TextLabel_1.TextSize = 14
			TextLabel_1.Size = UDim2.new(1.00, 0.00, 1.00, 0.00)
			TextLabel_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			TextLabel_1.Text = "Claim"
			TextLabel_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			TextLabel_1.BackgroundTransparency = 1
			TextLabel_1.Parent = SurfaceGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 4
			UIStroke_1.Parent = TextLabel_1

			local Claimed_1 = Instance.new("StringValue")
			Claimed_1.Name = "Claimed"
			Claimed_1.Value = "None"
			Claimed_1.Parent = __1

			local Upgrades_1 = Instance.new("Folder")
			Upgrades_1.Name = "Upgrades"
			Upgrades_1.Parent = __1

			local Buttons_1 = Instance.new("Folder")
			Buttons_1.Name = "Buttons"
			Buttons_1.Parent = __1

			local RobuxButtons_1 = Instance.new("Folder")
			RobuxButtons_1.Name = "RobuxButtons"
			RobuxButtons_1.Parent = __1

			--WORPLACE Script "README" (Disabled)
	--[[
	--=MORE UPGRADES=--
	Go to: ReplicatedStorage > TemplatePlot,
	then select the thing u want as an upgrade and move it in:
	ReplicatedStorage > TemplatePlot > Upgrades,
	then go to:
	ReplicatedStorage > TemplatePlot > Buttons,
	select one of those buttons and duplicate it (CTRL + D)
		And name it (example 2) and same with the upgrade
	--=GAMEPASSIDS=--
	Go to: ReplicatedStorage > GamepassIds, then 
	copy your id and change the number to your gamepass id
	--=RESET DATA=--
	Go to: ReplicatedStorage > Game Settings > Datasave and change the number to (example: PlayerData5964668)
	--=CHANGE REBIRTH PRICE=--
	Go to: ReplicatedStorage > Game Settings > Balancing > RebirthPrice and change the cost to what you want
	--=ADD MORE TOOLS=--
	Go to: ServerScriptService > RobuxHandler, then put in the tool u want to be in shop,
	now go to ReplicatedStorage > GamePassIds, duplicate one of those values (CTRL + D),
	name it exactly as the tool and change the number to the id of the tool
	]]


			--WORKPLACE "Spawn Location"
			local SpawnLocation = Instance.new("SpawnLocation")
			SpawnLocation.Anchored = true
			SpawnLocation.BottomSurface = Enum.SurfaceType.Smooth
			SpawnLocation.Duration = 0
			SpawnLocation.TopSurface = Enum.SurfaceType.Smooth
			SpawnLocation.Size = Vector3.new(12.00, 1.00, 12.00)
			SpawnLocation.CFrame = CFrame.new(0.00, 0.50, 0.00, -0.00, -0.00, -1.00)
			SpawnLocation.BrickColor = BrickColor.new("Medium stone grey")
			SpawnLocation.Position = Vector3.new(0.00, 0.50, 0.00)
			SpawnLocation.Parent = game:GetService("Workspace")


			From me: just so you know here is what i mean by how it looks from the code converter:

				--REPLICATED STORAGE (second photo as example) "GAME SETTINGS": 
				local Game_Settings = Instance.new("Folder")
			Game_Settings.Name = "Game Settings"
			Game_Settings.Parent = game:GetService("ReplicatedStorage")

			local GameType = Instance.new("StringValue")
			GameType.Name = "GameType"
			GameType.Value = "Classic"
			GameType.Parent = Game_Settings

			local DataSave = Instance.new("StringValue")
			DataSave.Name = "DataSave"
			DataSave.Value = "PlayerData172511086"
			DataSave.Parent = Game_Settings

			local Balancing = Instance.new("Folder")
			Balancing.Name = "Balancing"
			Balancing.Parent = Game_Settings

			local DefaultDropAmount = Instance.new("NumberValue")
			DefaultDropAmount.Name = "DefaultDropAmount"
			DefaultDropAmount.Value = 1
			DefaultDropAmount.Parent = Balancing

			local RebirthPrice = Instance.new("NumberValue")
			RebirthPrice.Name = "RebirthPrice"
			RebirthPrice.Value = 20000
			RebirthPrice.Parent = Balancing

			--REPLICATED STORAGE (second photo as example) "GAMEPASS ID's": 
				local GamepassIds = Instance.new("Folder")
			GamepassIds.Name = "GamepassIds"
			GamepassIds.Parent = game:GetService("ReplicatedStorage")

			local Sword = Instance.new("NumberValue")
			Sword.Name = "Sword"
			Sword.Value = 851326940
			Sword.Parent = GamepassIds

			local LaserGun = Instance.new("NumberValue")
			LaserGun.Name = "LaserGun"
			LaserGun.Value = 851546191
			LaserGun.Parent = GamepassIds

			local GravityCoil = Instance.new("NumberValue")
			GravityCoil.Name = "GravityCoil"
			GravityCoil.Value = 851492400
			GravityCoil.Parent = GamepassIds

			local SpeedCoil = Instance.new("NumberValue")
			SpeedCoil.Name = "SpeedCoil"
			SpeedCoil.Value = 851509295
			SpeedCoil.Parent = GamepassIds

			local DoubleMoney = Instance.new("NumberValue")
			DoubleMoney.Name = "DoubleMoney"
			DoubleMoney.Value = 933789599
			DoubleMoney.Parent = GamepassIds

			--REPLICATED STORAGE (second photo as example) "REMOTE EVENTS": 
				local RemoteEvents = Instance.new("Folder")
			RemoteEvents.Name = "RemoteEvents"
			RemoteEvents.Parent = game:GetService("ReplicatedStorage")

			local BuyRebirth = Instance.new("RemoteEvent")
			BuyRebirth.Name = "BuyRebirth"
			BuyRebirth.Parent = RemoteEvents

			--REPLICATED STORAGE (second photo as example) "TEMPLATE PLOT": 
				local TemplatePlot = Instance.new("Folder")
			TemplatePlot.Name = "TemplatePlot"
			TemplatePlot.Parent = game:GetService("ReplicatedStorage")

			local Ground = Instance.new("Part")
			Ground.Name = "Ground"
			Ground.TopSurface = Enum.SurfaceType.Smooth
			Ground.Color = Color3.new(0.55, 0.55, 0.55)
			Ground.Anchored = true
			Ground.Size = Vector3.new(50.00, 0.50, 50.00)
			Ground.BottomSurface = Enum.SurfaceType.Smooth
			Ground.BrickColor = BrickColor.new("Silver flip/flop")
			Ground.Position = Vector3.new(0.00, 15.75, 0.00)
			Ground.CFrame = CFrame.new(0.00, 15.75, 0.00, -0.00, -0.00, -1.00)
			Ground.Parent = TemplatePlot

			local Texture = Instance.new("Texture")
			Texture.Face = Enum.NormalId.Top
			Texture.StudsPerTileU = 5
			Texture.Transparency = 0.9599999785423279
			Texture.StudsPerTileV = 5
			Texture.Texture = "rbxassetid://6794119868"
			Texture.Parent = Ground

			local Door = Instance.new("Model")
			Door.Name = "Door"
			Door.WorldPivot = CFrame.new(0.00, 19.50, 24.00, -0.00, -0.00, -1.00)
			Door.Parent = TemplatePlot

			local Door_1 = Instance.new("Part")
			Door_1.Name = "Door"
			Door_1.TopSurface = Enum.SurfaceType.Smooth
			Door_1.Color = Color3.new(0.21, 0.21, 0.21)
			Door_1.Anchored = true
			Door_1.Size = Vector3.new(6.00, 1.00, 1.00)
			Door_1.BottomSurface = Enum.SurfaceType.Smooth
			Door_1.BrickColor = BrickColor.new("Black")
			Door_1.Position = Vector3.new(0.00, 23.50, 24.50)
			Door_1.CFrame = CFrame.new(0.00, 23.50, 24.50, -0.00, -0.00, -1.00)
			Door_1.Parent = Door

			local Door_1 = Instance.new("Part")
			Door_1.Name = "Door"
			Door_1.TopSurface = Enum.SurfaceType.Smooth
			Door_1.Color = Color3.new(0.21, 0.21, 0.21)
			Door_1.Anchored = true
			Door_1.Size = Vector3.new(1.00, 8.00, 1.00)
			Door_1.BottomSurface = Enum.SurfaceType.Smooth
			Door_1.BrickColor = BrickColor.new("Black")
			Door_1.Position = Vector3.new(-3.50, 20.00, 24.50)
			Door_1.CFrame = CFrame.new(-3.50, 20.00, 24.50, -0.00, -0.00, -1.00)
			Door_1.Parent = Door

			local Door_1 = Instance.new("Part")
			Door_1.Name = "Door"
			Door_1.TopSurface = Enum.SurfaceType.Smooth
			Door_1.Color = Color3.new(0.21, 0.21, 0.21)
			Door_1.Anchored = true
			Door_1.Size = Vector3.new(1.00, 8.00, 1.00)
			Door_1.BottomSurface = Enum.SurfaceType.Smooth
			Door_1.BrickColor = BrickColor.new("Black")
			Door_1.Position = Vector3.new(3.50, 20.00, 24.50)
			Door_1.CFrame = CFrame.new(3.50, 20.00, 24.50, -0.00, -0.00, -1.00)
			Door_1.Parent = Door

			local Claim = Instance.new("Part")
			Claim.Name = "Claim"
			Claim.TopSurface = Enum.SurfaceType.Smooth
			Claim.Color = Color3.new(0.55, 0.55, 0.55)
			Claim.Anchored = true
			Claim.Size = Vector3.new(6.00, 7.00, 0.50)
			Claim.BottomSurface = Enum.SurfaceType.Smooth
			Claim.CanCollide = false
			Claim.Rotation = Vector3.new(180.00, 0.00, 180.00)
			Claim.Transparency = 0.25
			Claim.BrickColor = BrickColor.new("Silver flip/flop")
			Claim.Position = Vector3.new(0.00, 19.50, 24.50)
			Claim.CFrame = CFrame.new(0.00, 19.50, 24.50, 0.00, -0.00, 1.00)
			Claim.Parent = Door

			local SurfaceGui = Instance.new("SurfaceGui")
			SurfaceGui.LightInfluence = 1
			SurfaceGui.SizingMode = Enum.SurfaceGuiSizingMode.PixelsPerStud
			SurfaceGui.AlwaysOnTop = true
			SurfaceGui.ClipsDescendants = true
			SurfaceGui.MaxDistance = 1000
			SurfaceGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
			SurfaceGui.Parent = Claim

			local TextLabel = Instance.new("TextLabel")
			TextLabel.TextWrapped = true
			TextLabel.BorderSizePixel = 0
			TextLabel.TextScaled = true
			TextLabel.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			TextLabel.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			TextLabel.TextSize = 14
			TextLabel.Size = UDim2.new(1.00, 0.00, 1.00, 0.00)
			TextLabel.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			TextLabel.Text = "Claim"
			TextLabel.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			TextLabel.BackgroundTransparency = 1
			TextLabel.Parent = SurfaceGui

			local UIStroke = Instance.new("UIStroke")
			UIStroke.Thickness = 4
			UIStroke.Parent = TextLabel

			local Buttons = Instance.new("Folder")
			Buttons.Name = "Buttons"
			Buttons.Parent = TemplatePlot

			local _ = Instance.new("Part")
			_.Name = "2"
			_.TopSurface = Enum.SurfaceType.Smooth
			_.Color = Color3.new(1.00, 0.14, 0.14)
			_.Shape = Enum.PartType.Cylinder
			_.Anchored = true
			_.Size = Vector3.new(0.50, 3.50, 3.50)
			_.BottomSurface = Enum.SurfaceType.Smooth
			_.Rotation = Vector3.new(-90.00, 90.00, 0.00)
			_.BrickColor = BrickColor.new("Really red")
			_.Position = Vector3.new(19.00, 16.25, 8.00)
			_.CFrame = CFrame.new(19.00, 16.25, 8.00, -1.00, -0.00, -0.00)
			_.Parent = Buttons

			local BillboardGui = Instance.new("BillboardGui")
			BillboardGui.Active = true
			BillboardGui.Size = UDim2.new(4.00, 0.00, 1.00, 0.00)
			BillboardGui.ClipsDescendants = true
			BillboardGui.MaxDistance = 100
			BillboardGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
			BillboardGui.StudsOffset = Vector3.new(0.00, 1.50, 0.00)
			BillboardGui.Parent = _

			local Price = Instance.new("TextLabel")
			Price.Name = "Price"
			Price.TextWrapped = true
			Price.BorderSizePixel = 0
			Price.TextScaled = true
			Price.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Price.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Price.TextSize = 14
			Price.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Price.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Price.Text = "$100"
			Price.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Price.BackgroundTransparency = 1
			Price.Position = UDim2.new(0.00, 0.00, 0.50, 0.00)
			Price.Parent = BillboardGui

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Price

			local Item = Instance.new("TextLabel")
			Item.Name = "Item"
			Item.TextWrapped = true
			Item.BorderSizePixel = 0
			Item.TextScaled = true
			Item.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Item.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Item.TextSize = 14
			Item.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Item.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Item.Text = "Start Working!"
			Item.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Item.BackgroundTransparency = 1
			Item.Parent = BillboardGui

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Item

			local Price_1 = Instance.new("IntValue")
			Price_1.Name = "Price"
			Price_1.Parent = _

			local UnlockedByButton = Instance.new("IntValue")
			UnlockedByButton.Name = "UnlockedByButton"
			UnlockedByButton.Value = 1
			UnlockedByButton.Parent = _

			local __1 = Instance.new("Part")
			__1.Name = "1"
			__1.TopSurface = Enum.SurfaceType.Smooth
			__1.Color = Color3.new(1.00, 0.14, 0.14)
			__1.Shape = Enum.PartType.Cylinder
			__1.Anchored = true
			__1.Size = Vector3.new(0.50, 3.50, 3.50)
			__1.BottomSurface = Enum.SurfaceType.Smooth
			__1.Rotation = Vector3.new(-90.00, 90.00, 0.00)
			__1.BrickColor = BrickColor.new("Really red")
			__1.Position = Vector3.new(11.00, 16.25, 8.29)
			__1.CFrame = CFrame.new(11.00, 16.25, 8.29, -1.00, -0.00, -0.00)
			__1.Parent = Buttons

			local BillboardGui_1 = Instance.new("BillboardGui")
			BillboardGui_1.Active = true
			BillboardGui_1.Size = UDim2.new(4.00, 0.00, 1.00, 0.00)
			BillboardGui_1.ClipsDescendants = true
			BillboardGui_1.MaxDistance = 100
			BillboardGui_1.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
			BillboardGui_1.StudsOffset = Vector3.new(0.00, 1.50, 0.00)
			BillboardGui_1.Parent = __1

			local Price_1 = Instance.new("TextLabel")
			Price_1.Name = "Price"
			Price_1.TextWrapped = true
			Price_1.BorderSizePixel = 0
			Price_1.TextScaled = true
			Price_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Price_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Price_1.TextSize = 14
			Price_1.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Price_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Price_1.Text = "$100"
			Price_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Price_1.BackgroundTransparency = 1
			Price_1.Position = UDim2.new(0.00, 0.00, 0.50, 0.00)
			Price_1.Parent = BillboardGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Price_1

			local Item_1 = Instance.new("TextLabel")
			Item_1.Name = "Item"
			Item_1.TextWrapped = true
			Item_1.BorderSizePixel = 0
			Item_1.TextScaled = true
			Item_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Item_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Item_1.TextSize = 14
			Item_1.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Item_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Item_1.Text = "Get Started!"
			Item_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Item_1.BackgroundTransparency = 1
			Item_1.Parent = BillboardGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Item_1

			local Price_1 = Instance.new("IntValue")
			Price_1.Name = "Price"
			Price_1.Parent = __1

			local UnlockedByButton_1 = Instance.new("IntValue")
			UnlockedByButton_1.Name = "UnlockedByButton"
			UnlockedByButton_1.Parent = __1

			local __1 = Instance.new("Part")
			__1.Name = "3"
			__1.TopSurface = Enum.SurfaceType.Smooth
			__1.Color = Color3.new(1.00, 0.14, 0.14)
			__1.Shape = Enum.PartType.Cylinder
			__1.Anchored = true
			__1.Size = Vector3.new(0.50, 3.50, 3.50)
			__1.BottomSurface = Enum.SurfaceType.Smooth
			__1.Rotation = Vector3.new(-90.00, 90.00, 0.00)
			__1.BrickColor = BrickColor.new("Really red")
			__1.Position = Vector3.new(12.45, 16.25, -8.55)
			__1.CFrame = CFrame.new(12.45, 16.25, -8.55, -1.00, -0.00, -0.00)
			__1.Parent = Buttons

			local BillboardGui_1 = Instance.new("BillboardGui")
			BillboardGui_1.Active = true
			BillboardGui_1.Size = UDim2.new(4.00, 0.00, 1.00, 0.00)
			BillboardGui_1.ClipsDescendants = true
			BillboardGui_1.MaxDistance = 100
			BillboardGui_1.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
			BillboardGui_1.StudsOffset = Vector3.new(0.00, 1.50, 0.00)
			BillboardGui_1.Parent = __1

			local Price_1 = Instance.new("TextLabel")
			Price_1.Name = "Price"
			Price_1.TextWrapped = true
			Price_1.BorderSizePixel = 0
			Price_1.TextScaled = true
			Price_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Price_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Price_1.TextSize = 14
			Price_1.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Price_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Price_1.Text = "$100"
			Price_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Price_1.BackgroundTransparency = 1
			Price_1.Position = UDim2.new(0.00, 0.00, 0.50, 0.00)
			Price_1.Parent = BillboardGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Price_1

			local Item_1 = Instance.new("TextLabel")
			Item_1.Name = "Item"
			Item_1.TextWrapped = true
			Item_1.BorderSizePixel = 0
			Item_1.TextScaled = true
			Item_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Item_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Item_1.TextSize = 14
			Item_1.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Item_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Item_1.Text = "2nd Dropper"
			Item_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Item_1.BackgroundTransparency = 1
			Item_1.Parent = BillboardGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Item_1

			local Price_1 = Instance.new("IntValue")
			Price_1.Name = "Price"
			Price_1.Value = 5
			Price_1.Parent = __1

			local UnlockedByButton_1 = Instance.new("IntValue")
			UnlockedByButton_1.Name = "UnlockedByButton"
			UnlockedByButton_1.Value = 2
			UnlockedByButton_1.Parent = __1

			local __1 = Instance.new("Part")
			__1.Name = "4"
			__1.TopSurface = Enum.SurfaceType.Smooth
			__1.Color = Color3.new(1.00, 0.14, 0.14)
			__1.Shape = Enum.PartType.Cylinder
			__1.Anchored = true
			__1.Size = Vector3.new(0.50, 3.50, 3.50)
			__1.BottomSurface = Enum.SurfaceType.Smooth
			__1.Rotation = Vector3.new(-90.00, 90.00, 0.00)
			__1.BrickColor = BrickColor.new("Really red")
			__1.Position = Vector3.new(7.90, 16.25, -8.55)
			__1.CFrame = CFrame.new(7.90, 16.25, -8.55, -1.00, -0.00, -0.00)
			__1.Parent = Buttons

			local BillboardGui_1 = Instance.new("BillboardGui")
			BillboardGui_1.Active = true
			BillboardGui_1.Size = UDim2.new(4.00, 0.00, 1.00, 0.00)
			BillboardGui_1.ClipsDescendants = true
			BillboardGui_1.MaxDistance = 100
			BillboardGui_1.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
			BillboardGui_1.StudsOffset = Vector3.new(0.00, 1.50, 0.00)
			BillboardGui_1.Parent = __1

			local Price_1 = Instance.new("TextLabel")
			Price_1.Name = "Price"
			Price_1.TextWrapped = true
			Price_1.BorderSizePixel = 0
			Price_1.TextScaled = true
			Price_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Price_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Price_1.TextSize = 14
			Price_1.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Price_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Price_1.Text = "$100"
			Price_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Price_1.BackgroundTransparency = 1
			Price_1.Position = UDim2.new(0.00, 0.00, 0.50, 0.00)
			Price_1.Parent = BillboardGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Price_1

			local Item_1 = Instance.new("TextLabel")
			Item_1.Name = "Item"
			Item_1.TextWrapped = true
			Item_1.BorderSizePixel = 0
			Item_1.TextScaled = true
			Item_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Item_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Item_1.TextSize = 14
			Item_1.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Item_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Item_1.Text = "3rd Dropper"
			Item_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Item_1.BackgroundTransparency = 1
			Item_1.Parent = BillboardGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Item_1

			local Price_1 = Instance.new("IntValue")
			Price_1.Name = "Price"
			Price_1.Value = 15
			Price_1.Parent = __1

			local UnlockedByButton_1 = Instance.new("IntValue")
			UnlockedByButton_1.Name = "UnlockedByButton"
			UnlockedByButton_1.Value = 3
			UnlockedByButton_1.Parent = __1

			local __1 = Instance.new("Part")
			__1.Name = "5"
			__1.TopSurface = Enum.SurfaceType.Smooth
			__1.Color = Color3.new(1.00, 0.14, 0.14)
			__1.Shape = Enum.PartType.Cylinder
			__1.Anchored = true
			__1.Size = Vector3.new(0.50, 3.50, 3.50)
			__1.BottomSurface = Enum.SurfaceType.Smooth
			__1.Rotation = Vector3.new(-90.00, 90.00, 0.00)
			__1.BrickColor = BrickColor.new("Really red")
			__1.Position = Vector3.new(7.90, 16.25, 21.45)
			__1.CFrame = CFrame.new(7.90, 16.25, 21.45, -1.00, -0.00, -0.00)
			__1.Parent = Buttons

			local BillboardGui_1 = Instance.new("BillboardGui")
			BillboardGui_1.Active = true
			BillboardGui_1.Size = UDim2.new(4.00, 0.00, 1.00, 0.00)
			BillboardGui_1.ClipsDescendants = true
			BillboardGui_1.MaxDistance = 100
			BillboardGui_1.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
			BillboardGui_1.StudsOffset = Vector3.new(0.00, 1.50, 0.00)
			BillboardGui_1.Parent = __1
			local Price_1 = Instance.new("TextLabel")
			Price_1.Name = "Price"
			Price_1.TextWrapped = true
			Price_1.BorderSizePixel = 0
			Price_1.TextScaled = true
			Price_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Price_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Price_1.TextSize = 14
			Price_1.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Price_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Price_1.Text = "$25"
			Price_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Price_1.BackgroundTransparency = 1
			Price_1.Position = UDim2.new(0.00, 0.00, 0.50, 0.00)
			Price_1.Parent = BillboardGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Price_1

			local Item_1 = Instance.new("TextLabel")
			Item_1.Name = "Item"
			Item_1.TextWrapped = true
			Item_1.BorderSizePixel = 0
			Item_1.TextScaled = true
			Item_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Item_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Item_1.TextSize = 14
			Item_1.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Item_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Item_1.Text = "Walls"
			Item_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Item_1.BackgroundTransparency = 1
			Item_1.Parent = BillboardGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Item_1

			local Price_1 = Instance.new("IntValue")
			Price_1.Name = "Price"
			Price_1.Value = 25
			Price_1.Parent = __1

			local UnlockedByButton_1 = Instance.new("IntValue")
			UnlockedByButton_1.Name = "UnlockedByButton"
			UnlockedByButton_1.Value = 2
			UnlockedByButton_1.Parent = __1

			local __1 = Instance.new("Part")
			__1.Name = "6"
			__1.TopSurface = Enum.SurfaceType.Smooth
			__1.Color = Color3.new(1.00, 0.14, 0.14)
			__1.Shape = Enum.PartType.Cylinder
			__1.Anchored = true
			__1.Size = Vector3.new(0.50, 3.50, 3.50)
			__1.BottomSurface = Enum.SurfaceType.Smooth
			__1.Rotation = Vector3.new(-90.00, 90.00, 0.00)
			__1.BrickColor = BrickColor.new("Really red")
			__1.Position = Vector3.new(-13.10, 16.25, 5.00)
			__1.CFrame = CFrame.new(-13.10, 16.25, 5.00, -1.00, -0.00, -0.00)
			__1.Parent = Buttons

			local BillboardGui_1 = Instance.new("BillboardGui")
			BillboardGui_1.Active = true
			BillboardGui_1.Size = UDim2.new(4.00, 0.00, 1.00, 0.00)
			BillboardGui_1.ClipsDescendants = true
			BillboardGui_1.MaxDistance = 100
			BillboardGui_1.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
			BillboardGui_1.StudsOffset = Vector3.new(0.00, 1.50, 0.00)
			BillboardGui_1.Parent = __1

			local Price_1 = Instance.new("TextLabel")
			Price_1.Name = "Price"
			Price_1.TextWrapped = true
			Price_1.BorderSizePixel = 0
			Price_1.TextScaled = true
			Price_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Price_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Price_1.TextSize = 14
			Price_1.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Price_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Price_1.Text = "$25"
			Price_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Price_1.BackgroundTransparency = 1
			Price_1.Position = UDim2.new(0.00, 0.00, 0.50, 0.00)
			Price_1.Parent = BillboardGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Price_1

			local Item_1 = Instance.new("TextLabel")
			Item_1.Name = "Item"
			Item_1.TextWrapped = true
			Item_1.BorderSizePixel = 0
			Item_1.TextScaled = true
			Item_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Item_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Item_1.TextSize = 14
			Item_1.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Item_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Item_1.Text = "Conveyor Walls"
			Item_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Item_1.BackgroundTransparency = 1
			Item_1.Parent = BillboardGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Item_1

			local Price_1 = Instance.new("IntValue")
			Price_1.Name = "Price"
			Price_1.Value = 35
			Price_1.Parent = __1

			local UnlockedByButton_1 = Instance.new("IntValue")
			UnlockedByButton_1.Name = "UnlockedByButton"
			UnlockedByButton_1.Value = 3
			UnlockedByButton_1.Parent = __1

			local __1 = Instance.new("Part")
			__1.Name = "7"
			__1.TopSurface = Enum.SurfaceType.Smooth
			__1.Color = Color3.new(1.00, 0.14, 0.14)
			__1.Shape = Enum.PartType.Cylinder
			__1.Anchored = true
			__1.Size = Vector3.new(0.50, 3.50, 3.50)
			__1.BottomSurface = Enum.SurfaceType.Smooth
			__1.Rotation = Vector3.new(-90.00, 90.00, 0.00)
			__1.BrickColor = BrickColor.new("Really red")
			__1.Position = Vector3.new(2.90, 16.25, -8.55)
			__1.CFrame = CFrame.new(2.90, 16.25, -8.55, -1.00, -0.00, -0.00)
			__1.Parent = Buttons

			local BillboardGui_1 = Instance.new("BillboardGui")
			BillboardGui_1.Active = true
			BillboardGui_1.Size = UDim2.new(4.00, 0.00, 1.00, 0.00)
			BillboardGui_1.ClipsDescendants = true
			BillboardGui_1.MaxDistance = 100
			BillboardGui_1.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
			BillboardGui_1.StudsOffset = Vector3.new(0.00, 1.50, 0.00)
			BillboardGui_1.Parent = __1

			local Price_1 = Instance.new("TextLabel")
			Price_1.Name = "Price"
			Price_1.TextWrapped = true
			Price_1.BorderSizePixel = 0
			Price_1.TextScaled = true
			Price_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Price_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Price_1.TextSize = 14
			Price_1.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Price_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Price_1.Text = "$100"
			Price_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Price_1.BackgroundTransparency = 1
			Price_1.Position = UDim2.new(0.00, 0.00, 0.50, 0.00)
			Price_1.Parent = BillboardGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Price_1

			local Item_1 = Instance.new("TextLabel")
			Item_1.Name = "Item"
			Item_1.TextWrapped = true
			Item_1.BorderSizePixel = 0
			Item_1.TextScaled = true
			Item_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Item_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Item_1.TextSize = 14
			Item_1.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Item_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Item_1.Text = "4th Dropper"
			Item_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Item_1.BackgroundTransparency = 1
			Item_1.Parent = BillboardGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Item_1

			local Price_1 = Instance.new("IntValue")
			Price_1.Name = "Price"
			Price_1.Value = 30
			Price_1.Parent = __1

			local UnlockedByButton_1 = Instance.new("IntValue")
			UnlockedByButton_1.Name = "UnlockedByButton"
			UnlockedByButton_1.Value = 4
			UnlockedByButton_1.Parent = __1

			local __1 = Instance.new("Part")
			__1.Name = "8"
			__1.TopSurface = Enum.SurfaceType.Smooth
			__1.Color = Color3.new(1.00, 0.14, 0.14)
			__1.Shape = Enum.PartType.Cylinder
			__1.Anchored = true
			__1.Size = Vector3.new(0.50, 3.50, 3.50)
			__1.BottomSurface = Enum.SurfaceType.Smooth
			__1.Rotation = Vector3.new(-90.00, 90.00, 0.00)
			__1.BrickColor = BrickColor.new("Really red")
			__1.Position = Vector3.new(12.40, 16.25, 21.45)
			__1.CFrame = CFrame.new(12.40, 16.25, 21.45, -1.00, -0.00, -0.00)
			__1.Parent = Buttons

			local BillboardGui_1 = Instance.new("BillboardGui")
			BillboardGui_1.Active = true
			BillboardGui_1.Size = UDim2.new(4.00, 0.00, 1.00, 0.00)
			BillboardGui_1.ClipsDescendants = true
			BillboardGui_1.MaxDistance = 100
			BillboardGui_1.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
			BillboardGui_1.StudsOffset = Vector3.new(0.00, 1.50, 0.00)
			BillboardGui_1.Parent = __1

			local Price_1 = Instance.new("TextLabel")
			Price_1.Name = "Price"
			Price_1.TextWrapped = true
			Price_1.BorderSizePixel = 0
			Price_1.TextScaled = true
			Price_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Price_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Price_1.TextSize = 14
			Price_1.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Price_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Price_1.Text = "$25"
			Price_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Price_1.BackgroundTransparency = 1
			Price_1.Position = UDim2.new(0.00, 0.00, 0.50, 0.00)
			Price_1.Parent = BillboardGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Price_1

			local Item_1 = Instance.new("TextLabel")
			Item_1.Name = "Item"
			Item_1.TextWrapped = true
			Item_1.BorderSizePixel = 0
			Item_1.TextScaled = true
			Item_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Item_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Item_1.TextSize = 14
			Item_1.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Item_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Item_1.Text = "Upgrade Walls"
			Item_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Item_1.BackgroundTransparency = 1
			Item_1.Parent = BillboardGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Item_1

			local Price_1 = Instance.new("IntValue")
			Price_1.Name = "Price"
			Price_1.Value = 75
			Price_1.Parent = __1

			local UnlockedByButton_1 = Instance.new("IntValue")
			UnlockedByButton_1.Name = "UnlockedByButton"
			UnlockedByButton_1.Value = 5
			UnlockedByButton_1.Parent = __1

			local __1 = Instance.new("Part")
			__1.Name = "9"
			__1.TopSurface = Enum.SurfaceType.Smooth
			__1.Color = Color3.new(1.00, 0.14, 0.14)
			__1.Shape = Enum.PartType.Cylinder
			__1.Anchored = true
			__1.Size = Vector3.new(0.50, 3.50, 3.50)
			__1.BottomSurface = Enum.SurfaceType.Smooth
			__1.Rotation = Vector3.new(-90.00, 90.00, 0.00)
			__1.BrickColor = BrickColor.new("Really red")
			__1.Position = Vector3.new(14.90, 16.25, 8.45)
			__1.CFrame = CFrame.new(14.90, 16.25, 8.45, -1.00, -0.00, -0.00)
			__1.Parent = Buttons

			local BillboardGui_1 = Instance.new("BillboardGui")
			BillboardGui_1.Active = true
			BillboardGui_1.Size = UDim2.new(4.00, 0.00, 1.00, 0.00)
			BillboardGui_1.ClipsDescendants = true
			BillboardGui_1.MaxDistance = 100
			BillboardGui_1.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
			BillboardGui_1.StudsOffset = Vector3.new(0.00, 1.50, 0.00)
			BillboardGui_1.Parent = __1

			local Price_1 = Instance.new("TextLabel")
			Price_1.Name = "Price"
			Price_1.TextWrapped = true
			Price_1.BorderSizePixel = 0
			Price_1.TextScaled = true
			Price_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Price_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Price_1.TextSize = 14
			Price_1.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Price_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Price_1.Text = "$100"
			Price_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Price_1.BackgroundTransparency = 1
			Price_1.Position = UDim2.new(0.00, 0.00, 0.50, 0.00)
			Price_1.Parent = BillboardGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Price_1

			local Item_1 = Instance.new("TextLabel")
			Item_1.Name = "Item"
			Item_1.TextWrapped = true
			Item_1.BorderSizePixel = 0
			Item_1.TextScaled = true
			Item_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Item_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Item_1.TextSize = 14
			Item_1.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Item_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Item_1.Text = "5th Dropper"
			Item_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Item_1.BackgroundTransparency = 1
			Item_1.Parent = BillboardGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Item_1

			local Price_1 = Instance.new("IntValue")
			Price_1.Name = "Price"
			Price_1.Value = 30
			Price_1.Parent = __1

			local UnlockedByButton_1 = Instance.new("IntValue")
			UnlockedByButton_1.Name = "UnlockedByButton"
			UnlockedByButton_1.Value = 4
			UnlockedByButton_1.Parent = __1

			local _0 = Instance.new("Part")
			_0.Name = "10"
			_0.TopSurface = Enum.SurfaceType.Smooth
			_0.Color = Color3.new(1.00, 0.14, 0.14)
			_0.Shape = Enum.PartType.Cylinder
			_0.Anchored = true
			_0.Size = Vector3.new(0.50, 3.50, 3.50)
			_0.BottomSurface = Enum.SurfaceType.Smooth
			_0.Rotation = Vector3.new(-90.00, 90.00, 0.00)
			_0.BrickColor = BrickColor.new("Really red")
			_0.Position = Vector3.new(16.40, 16.25, 21.45)
			_0.CFrame = CFrame.new(16.40, 16.25, 21.45, -1.00, -0.00, -0.00)
			_0.Parent = Buttons

			local BillboardGui_1 = Instance.new("BillboardGui")
			BillboardGui_1.Active = true
			BillboardGui_1.Size = UDim2.new(4.00, 0.00, 1.00, 0.00)
			BillboardGui_1.ClipsDescendants = true
			BillboardGui_1.MaxDistance = 100
			BillboardGui_1.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
			BillboardGui_1.StudsOffset = Vector3.new(0.00, 1.50, 0.00)
			BillboardGui_1.Parent = _0

			local Price_1 = Instance.new("TextLabel")
			Price_1.Name = "Price"
			Price_1.TextWrapped = true
			Price_1.BorderSizePixel = 0
			Price_1.TextScaled = true
			Price_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Price_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Price_1.TextSize = 14
			Price_1.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Price_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Price_1.Text = "$25"
			Price_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Price_1.BackgroundTransparency = 1
			Price_1.Position = UDim2.new(0.00, 0.00, 0.50, 0.00)
			Price_1.Parent = BillboardGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Price_1

			local Item_1 = Instance.new("TextLabel")
			Item_1.Name = "Item"
			Item_1.TextWrapped = true
			Item_1.BorderSizePixel = 0
			Item_1.TextScaled = true
			Item_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Item_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Item_1.TextSize = 14
			Item_1.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Item_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Item_1.Text = "Upgrade Walls"
			Item_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Item_1.BackgroundTransparency = 1
			Item_1.Parent = BillboardGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Item_1

			local Price_1 = Instance.new("IntValue")
			Price_1.Name = "Price"
			Price_1.Value = 125
			Price_1.Parent = _0

			local UnlockedByButton_1 = Instance.new("IntValue")
			UnlockedByButton_1.Name = "UnlockedByButton"
			UnlockedByButton_1.Value = 8
			UnlockedByButton_1.Parent = _0

			local _1 = Instance.new("Part")
			_1.Name = "11"
			_1.TopSurface = Enum.SurfaceType.Smooth
			_1.Color = Color3.new(1.00, 0.14, 0.14)
			_1.Shape = Enum.PartType.Cylinder
			_1.Anchored = true
			_1.Size = Vector3.new(0.50, 3.50, 3.50)
			_1.BottomSurface = Enum.SurfaceType.Smooth
			_1.Rotation = Vector3.new(-90.00, 90.00, 0.00)
			_1.BrickColor = BrickColor.new("Really red")
			_1.Position = Vector3.new(-6.60, 16.25, 21.45)
			_1.CFrame = CFrame.new(-6.60, 16.25, 21.45, -1.00, -0.00, -0.00)
			_1.Parent = Buttons
			local BillboardGui_1 = Instance.new("BillboardGui")
			BillboardGui_1.Active = true
			BillboardGui_1.Size = UDim2.new(4.00, 0.00, 1.00, 0.00)
			BillboardGui_1.ClipsDescendants = true
			BillboardGui_1.MaxDistance = 100
			BillboardGui_1.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
			BillboardGui_1.StudsOffset = Vector3.new(0.00, 1.50, 0.00)
			BillboardGui_1.Parent = _1

			local Price_1 = Instance.new("TextLabel")
			Price_1.Name = "Price"
			Price_1.TextWrapped = true
			Price_1.BorderSizePixel = 0
			Price_1.TextScaled = true
			Price_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Price_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Price_1.TextSize = 14
			Price_1.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Price_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Price_1.Text = "$25"
			Price_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Price_1.BackgroundTransparency = 1
			Price_1.Position = UDim2.new(0.00, 0.00, 0.50, 0.00)
			Price_1.Parent = BillboardGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Price_1

			local Item_1 = Instance.new("TextLabel")
			Item_1.Name = "Item"
			Item_1.TextWrapped = true
			Item_1.BorderSizePixel = 0
			Item_1.TextScaled = true
			Item_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Item_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Item_1.TextSize = 14
			Item_1.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Item_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Item_1.Text = "Second Floor"
			Item_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Item_1.BackgroundTransparency = 1
			Item_1.Parent = BillboardGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Item_1

			local Price_1 = Instance.new("IntValue")
			Price_1.Name = "Price"
			Price_1.Value = 150
			Price_1.Parent = _1

			local UnlockedByButton_1 = Instance.new("IntValue")
			UnlockedByButton_1.Name = "UnlockedByButton"
			UnlockedByButton_1.Value = 10
			UnlockedByButton_1.Parent = _1

			local _2 = Instance.new("Part")
			_2.Name = "12"
			_2.TopSurface = Enum.SurfaceType.Smooth
			_2.Color = Color3.new(1.00, 0.14, 0.14)
			_2.Shape = Enum.PartType.Cylinder
			_2.Anchored = true
			_2.Size = Vector3.new(0.50, 3.50, 3.50)
			_2.BottomSurface = Enum.SurfaceType.Smooth
			_2.Rotation = Vector3.new(-90.00, 90.00, 0.00)
			_2.BrickColor = BrickColor.new("Really red")
			_2.Position = Vector3.new(-11.60, 16.25, 21.45)
			_2.CFrame = CFrame.new(-11.60, 16.25, 21.45, -1.00, -0.00, -0.00)
			_2.Parent = Buttons

			local BillboardGui_1 = Instance.new("BillboardGui")
			BillboardGui_1.Active = true
			BillboardGui_1.Size = UDim2.new(4.00, 0.00, 1.00, 0.00)
			BillboardGui_1.ClipsDescendants = true
			BillboardGui_1.MaxDistance = 100
			BillboardGui_1.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
			BillboardGui_1.StudsOffset = Vector3.new(0.00, 1.50, 0.00)
			BillboardGui_1.Parent = _2

			local Price_1 = Instance.new("TextLabel")
			Price_1.Name = "Price"
			Price_1.TextWrapped = true
			Price_1.BorderSizePixel = 0
			Price_1.TextScaled = true
			Price_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Price_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Price_1.TextSize = 14
			Price_1.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Price_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Price_1.Text = "$25"
			Price_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Price_1.BackgroundTransparency = 1
			Price_1.Position = UDim2.new(0.00, 0.00, 0.50, 0.00)
			Price_1.Parent = BillboardGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Price_1

			local Item_1 = Instance.new("TextLabel")
			Item_1.Name = "Item"
			Item_1.TextWrapped = true
			Item_1.BorderSizePixel = 0
			Item_1.TextScaled = true
			Item_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Item_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Item_1.TextSize = 14
			Item_1.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Item_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Item_1.Text = "Stairs"
			Item_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Item_1.BackgroundTransparency = 1
			Item_1.Parent = BillboardGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Item_1

			local Price_1 = Instance.new("IntValue")
			Price_1.Name = "Price"
			Price_1.Value = 175
			Price_1.Parent = _2

			local UnlockedByButton_1 = Instance.new("IntValue")
			UnlockedByButton_1.Name = "UnlockedByButton"
			UnlockedByButton_1.Value = 11
			UnlockedByButton_1.Parent = _2

			local _3 = Instance.new("Part")
			_3.Name = "13"
			_3.TopSurface = Enum.SurfaceType.Smooth
			_3.Color = Color3.new(1.00, 0.14, 0.14)
			_3.Shape = Enum.PartType.Cylinder
			_3.Anchored = true
			_3.Size = Vector3.new(0.50, 3.50, 3.50)
			_3.BottomSurface = Enum.SurfaceType.Smooth
			_3.Rotation = Vector3.new(-90.00, 90.00, 0.00)
			_3.BrickColor = BrickColor.new("Really red")
			_3.Position = Vector3.new(6.15, 16.25, 21.45)
			_3.CFrame = CFrame.new(6.15, 16.25, 21.45, -1.00, -0.00, -0.00)
			_3.Parent = Buttons

			local BillboardGui_1 = Instance.new("BillboardGui")
			BillboardGui_1.Active = true
			BillboardGui_1.Size = UDim2.new(4.00, 0.00, 1.00, 0.00)
			BillboardGui_1.ClipsDescendants = true
			BillboardGui_1.MaxDistance = 100
			BillboardGui_1.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
			BillboardGui_1.StudsOffset = Vector3.new(0.00, 1.50, 0.00)
			BillboardGui_1.Parent = _3

			local Price_1 = Instance.new("TextLabel")
			Price_1.Name = "Price"
			Price_1.TextWrapped = true
			Price_1.BorderSizePixel = 0
			Price_1.TextScaled = true
			Price_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Price_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Price_1.TextSize = 14
			Price_1.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Price_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Price_1.Text = "$500"
			Price_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Price_1.BackgroundTransparency = 1
			Price_1.Position = UDim2.new(0.00, 0.00, 0.50, 0.00)
			Price_1.Parent = BillboardGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Price_1

			local Item_1 = Instance.new("TextLabel")
			Item_1.Name = "Item"
			Item_1.TextWrapped = true
			Item_1.BorderSizePixel = 0
			Item_1.TextScaled = true
			Item_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Item_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Item_1.TextSize = 14
			Item_1.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Item_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Item_1.Text = "Laser Door"
			Item_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Item_1.BackgroundTransparency = 1
			Item_1.Parent = BillboardGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Item_1

			local Price_1 = Instance.new("IntValue")
			Price_1.Name = "Price"
			Price_1.Value = 500
			Price_1.Parent = _3

			local UnlockedByButton_1 = Instance.new("IntValue")
			UnlockedByButton_1.Name = "UnlockedByButton"
			UnlockedByButton_1.Value = 10
			UnlockedByButton_1.Parent = _3

			local _4 = Instance.new("Part")
			_4.Name = "14"
			_4.TopSurface = Enum.SurfaceType.Smooth
			_4.Color = Color3.new(1.00, 0.14, 0.14)
			_4.Shape = Enum.PartType.Cylinder
			_4.Anchored = true
			_4.Size = Vector3.new(0.50, 3.50, 3.50)
			_4.BottomSurface = Enum.SurfaceType.Smooth
			_4.Rotation = Vector3.new(-90.00, 90.00, 0.00)
			_4.BrickColor = BrickColor.new("Really red")
			_4.Position = Vector3.new(-5.85, 16.25, -5.80)
			_4.CFrame = CFrame.new(-5.85, 16.25, -5.80, -1.00, -0.00, -0.00)
			_4.Parent = Buttons

			local BillboardGui_1 = Instance.new("BillboardGui")
			BillboardGui_1.Active = true
			BillboardGui_1.Size = UDim2.new(4.00, 0.00, 1.00, 0.00)
			BillboardGui_1.ClipsDescendants = true
			BillboardGui_1.MaxDistance = 100
			BillboardGui_1.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
			BillboardGui_1.StudsOffset = Vector3.new(0.00, 1.50, 0.00)
			BillboardGui_1.Parent = _4

			local Price_1 = Instance.new("TextLabel")
			Price_1.Name = "Price"
			Price_1.TextWrapped = true
			Price_1.BorderSizePixel = 0
			Price_1.TextScaled = true
			Price_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Price_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Price_1.TextSize = 14
			Price_1.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Price_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Price_1.Text = "$500"
			Price_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Price_1.BackgroundTransparency = 1
			Price_1.Position = UDim2.new(0.00, 0.00, 0.50, 0.00)
			Price_1.Parent = BillboardGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Price_1

			local Item_1 = Instance.new("TextLabel")
			Item_1.Name = "Item"
			Item_1.TextWrapped = true
			Item_1.BorderSizePixel = 0
			Item_1.TextScaled = true
			Item_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Item_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Item_1.TextSize = 14
			Item_1.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Item_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Item_1.Text = "Upgrader"
			Item_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Item_1.BackgroundTransparency = 1
			Item_1.Parent = BillboardGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Item_1

			local Price_1 = Instance.new("IntValue")
			Price_1.Name = "Price"
			Price_1.Value = 1000
			Price_1.Parent = _4

			local UnlockedByButton_1 = Instance.new("IntValue")
			UnlockedByButton_1.Name = "UnlockedByButton"
			UnlockedByButton_1.Value = 9
			UnlockedByButton_1.Parent = _4

			local Upgrades = Instance.new("Folder")
			Upgrades.Name = "Upgrades"
			Upgrades.Parent = TemplatePlot

			local __1 = Instance.new("Model")
			__1.Name = "2"
			__1.WorldPivot = CFrame.new(17.50, 19.25, 0.00, -1.00, 0.00, -0.00)
			__1.Parent = Upgrades

			local Base = Instance.new("Part")
			Base.Name = "Base"
			Base.TopSurface = Enum.SurfaceType.Smooth
			Base.Color = Color3.new(0.44, 0.43, 0.44)
			Base.Anchored = true
			Base.Size = Vector3.new(3.00, 1.00, 3.00)
			Base.BottomSurface = Enum.SurfaceType.Smooth
			Base.Rotation = Vector3.new(0.00, 90.00, 0.00)
			Base.BrickColor = BrickColor.new("Dark grey")
			Base.Position = Vector3.new(19.25, 16.50, 0.00)
			Base.CFrame = CFrame.new(19.25, 16.50, 0.00, -1.00, 0.00, -0.00)
			Base.Parent = __1

			local Main = Instance.new("Part")
			Main.Name = "Main"
			Main.TopSurface = Enum.SurfaceType.Smooth
			Main.Color = Color3.new(0.53, 0.52, 0.53)
			Main.Anchored = true
			Main.Size = Vector3.new(2.00, 5.50, 2.00)
			Main.BottomSurface = Enum.SurfaceType.Smooth
			Main.Rotation = Vector3.new(0.00, 90.00, 0.00)
			Main.BrickColor = BrickColor.new("Silver flip/flop")
			Main.Position = Vector3.new(19.25, 19.75, 0.00)
			Main.CFrame = CFrame.new(19.25, 19.75, 0.00, -1.00, 0.00, -0.00)
			Main.Parent = __1

			local Arm = Instance.new("Part")
			Arm.Name = "Arm"
			Arm.TopSurface = Enum.SurfaceType.Smooth
			Arm.Color = Color3.new(0.44, 0.43, 0.44)
			Arm.Anchored = true
			Arm.Size = Vector3.new(1.50, 1.00, 4.00)
			Arm.BottomSurface = Enum.SurfaceType.Smooth
			Arm.Rotation = Vector3.new(0.00, 90.00, 0.00)
			Arm.BrickColor = BrickColor.new("Dark grey")
			Arm.Position = Vector3.new(16.25, 21.50, 0.00)
			Arm.CFrame = CFrame.new(16.25, 21.50, 0.00, -1.00, 0.00, -0.00)
			Arm.Parent = __1

			local Spawner = Instance.new("Part")
			Spawner.Name = "Spawner"
			Spawner.TopSurface = Enum.SurfaceType.Smooth
			Spawner.Color = Color3.new(0.44, 0.43, 0.44)
			Spawner.Anchored = true
			Spawner.Size = Vector3.new(0.75, 0.50, 0.75)
			Spawner.BottomSurface = Enum.SurfaceType.Smooth
			Spawner.Rotation = Vector3.new(0.00, 90.00, 0.00)
			Spawner.Transparency = 0.25
			Spawner.BrickColor = BrickColor.new("Dark grey")
			Spawner.Position = Vector3.new(15.00, 20.75, 0.00)
			Spawner.CFrame = CFrame.new(15.00, 20.75, 0.00, -1.00, 0.00, -0.00)
			Spawner.Parent = __1

			local Dropperscript = Instance.new("Script")
			Dropperscript.Name = "Dropperscript"
			Dropperscript.Source = "local Dropper\n\nfunction StartDropping()\n	local PlayerName = script.Parent.Parent.Parent.Parent.Claimed.Value\n	local Player = game.Players[PlayerName]\n\n	while task.wait(2) do\n		Dropper.Spawn(Player, script.Parent.Position + Vector3.new(0, -1, 0), script.Parent.Parent.DropAmount.Value)\n	end\nend\n\nrepeat task.wait(1) until script.Parent:IsDescendantOf(workspace)\nDropper = require(game.ServerScriptService:WaitForChild(\'Dropper\'))\nStartDropping()"
			Dropperscript.Parent = Spawner

			local DropAmount = Instance.new("NumberValue")
			DropAmount.Name = "DropAmount"
			DropAmount.Value = 2
			DropAmount.Parent = __1

			local __1 = Instance.new("Model")
			__1.Name = "1"
			__1.WorldPivot = CFrame.new(3.00, 16.25, 0.00, -0.00, -0.00, -1.00)
			__1.Parent = Upgrades

			local Conveyor = Instance.new("Part")
			Conveyor.Name = "Conveyor"
			Conveyor.TopSurface = Enum.SurfaceType.Smooth
			Conveyor.Color = Color3.new(0.37, 0.37, 0.37)
			Conveyor.Anchored = true
			Conveyor.Size = Vector3.new(23.85, 0.52, 4.15)
			Conveyor.BottomSurface = Enum.SurfaceType.Smooth
			Conveyor.AssemblyLinearVelocity = Vector3.new(-5.00, 0.00, 0.00)
			Conveyor.BrickColor = BrickColor.new("Dark stone grey")
			Conveyor.Position = Vector3.new(5.07, 16.25, 0.00)
			Conveyor.CFrame = CFrame.new(5.07, 16.25, 0.00, -0.00, -0.00, -1.00)
			Conveyor.Parent = __1

			local ConveyorScript = Instance.new("Script")
			ConveyorScript.Name = "ConveyorScript"
			ConveyorScript.Source = "local BaseVelocity = Vector3.new(-5 ,0, 0)\nlocal Conveyor = script.Parent\nConveyor.Velocity = Conveyor.CFrame:VectorToWorldSpace(BaseVelocity)"
			ConveyorScript.Parent = Conveyor

			local Furnace = Instance.new("Part")
			Furnace.Name = "Furnace"
			Furnace.TopSurface = Enum.SurfaceType.Smooth
			Furnace.Color = Color3.new(1.00, 0.15, 0.15)
			Furnace.Anchored = true
			Furnace.Size = Vector3.new(4.15, 0.52, 4.15)
			Furnace.BottomSurface = Enum.SurfaceType.Smooth
			Furnace.BrickColor = BrickColor.new("Bright red")
			Furnace.Position = Vector3.new(-8.93, 16.25, 0.00)
			Furnace.CFrame = CFrame.new(-8.93, 16.25, 0.00, -0.00, -0.00, -1.00)
			Furnace.Parent = __1

			local __1 = Instance.new("Model")
			__1.Name = "3"
			__1.WorldPivot = CFrame.new(12.25, 19.25, -3.21, -0.00, -0.00, 1.00)
			__1.Parent = Upgrades

			local Base_1 = Instance.new("Part")
			Base_1.Name = "Base"
			Base_1.TopSurface = Enum.SurfaceType.Smooth
			Base_1.Color = Color3.new(0.44, 0.43, 0.44)
			Base_1.Anchored = true
			Base_1.Size = Vector3.new(3.00, 1.00, 3.00)
			Base_1.BottomSurface = Enum.SurfaceType.Smooth
			Base_1.Rotation = Vector3.new(180.00, 0.00, 180.00)
			Base_1.BrickColor = BrickColor.new("Dark grey")
			Base_1.Position = Vector3.new(12.25, 16.50, -4.96)
			Base_1.CFrame = CFrame.new(12.25, 16.50, -4.96, -0.00, -0.00, 1.00)
			Base_1.Parent = __1
			local Main_1 = Instance.new("Part")
			Main_1.Name = "Main"
			Main_1.TopSurface = Enum.SurfaceType.Smooth
			Main_1.Color = Color3.new(0.53, 0.52, 0.53)
			Main_1.Anchored = true
			Main_1.Size = Vector3.new(2.00, 5.50, 2.00)
			Main_1.BottomSurface = Enum.SurfaceType.Smooth
			Main_1.Rotation = Vector3.new(180.00, 0.00, 180.00)
			Main_1.BrickColor = BrickColor.new("Silver flip/flop")
			Main_1.Position = Vector3.new(12.25, 19.75, -4.96)
			Main_1.CFrame = CFrame.new(12.25, 19.75, -4.96, -0.00, -0.00, 1.00)
			Main_1.Parent = __1

			local Arm_1 = Instance.new("Part")
			Arm_1.Name = "Arm"
			Arm_1.TopSurface = Enum.SurfaceType.Smooth
			Arm_1.Color = Color3.new(0.44, 0.43, 0.44)
			Arm_1.Anchored = true
			Arm_1.Size = Vector3.new(1.50, 1.00, 4.00)
			Arm_1.BottomSurface = Enum.SurfaceType.Smooth
			Arm_1.Rotation = Vector3.new(180.00, 0.00, 180.00)
			Arm_1.BrickColor = BrickColor.new("Dark grey")
			Arm_1.Position = Vector3.new(12.25, 21.50, -1.96)
			Arm_1.CFrame = CFrame.new(12.25, 21.50, -1.96, -0.00, -0.00, 1.00)
			Arm_1.Parent = __1

			local Spawner_1 = Instance.new("Part")
			Spawner_1.Name = "Spawner"
			Spawner_1.TopSurface = Enum.SurfaceType.Smooth
			Spawner_1.Color = Color3.new(0.44, 0.43, 0.44)
			Spawner_1.Anchored = true
			Spawner_1.Size = Vector3.new(0.75, 0.50, 0.75)
			Spawner_1.BottomSurface = Enum.SurfaceType.Smooth
			Spawner_1.Rotation = Vector3.new(180.00, 0.00, 180.00)
			Spawner_1.Transparency = 0.25
			Spawner_1.BrickColor = BrickColor.new("Dark grey")
			Spawner_1.Position = Vector3.new(12.25, 20.75, -0.71)
			Spawner_1.CFrame = CFrame.new(12.25, 20.75, -0.71, -0.00, -0.00, 1.00)
			Spawner_1.Parent = __1

			local Dropperscript_1 = Instance.new("Script")
			Dropperscript_1.Name = "Dropperscript"
			Dropperscript_1.Source = "local Dropper\n\nfunction StartDropping()\n	local PlayerName = script.Parent.Parent.Parent.Parent.Claimed.Value\n	local Player = game.Players[PlayerName]\n\n	while task.wait(2) do\n		Dropper.Spawn(Player, script.Parent.Position + Vector3.new(0, -1, 0), script.Parent.Parent.DropAmount.Value)\n	end\nend\n\nrepeat task.wait(1) until script.Parent:IsDescendantOf(workspace)\nDropper = require(game.ServerScriptService:WaitForChild(\'Dropper\'))\nStartDropping()"
			Dropperscript_1.Parent = Spawner_1

			local DropAmount_1 = Instance.new("NumberValue")
			DropAmount_1.Name = "DropAmount"
			DropAmount_1.Value = 2
			DropAmount_1.Parent = __1

			local __1 = Instance.new("Model")
			__1.Name = "4"
			__1.WorldPivot = CFrame.new(7.75, 19.25, -3.21, -0.00, -0.00, 1.00)
			__1.Parent = Upgrades

			local Base_1 = Instance.new("Part")
			Base_1.Name = "Base"
			Base_1.TopSurface = Enum.SurfaceType.Smooth
			Base_1.Color = Color3.new(0.44, 0.43, 0.44)
			Base_1.Anchored = true
			Base_1.Size = Vector3.new(3.00, 1.00, 3.00)
			Base_1.BottomSurface = Enum.SurfaceType.Smooth
			Base_1.Rotation = Vector3.new(180.00, 0.00, 180.00)
			Base_1.BrickColor = BrickColor.new("Dark grey")
			Base_1.Position = Vector3.new(7.75, 16.50, -4.96)
			Base_1.CFrame = CFrame.new(7.75, 16.50, -4.96, -0.00, -0.00, 1.00)
			Base_1.Parent = __1

			local Main_1 = Instance.new("Part")
			Main_1.Name = "Main"
			Main_1.TopSurface = Enum.SurfaceType.Smooth
			Main_1.Color = Color3.new(0.53, 0.52, 0.53)
			Main_1.Anchored = true
			Main_1.Size = Vector3.new(2.00, 5.50, 2.00)
			Main_1.BottomSurface = Enum.SurfaceType.Smooth
			Main_1.Rotation = Vector3.new(180.00, 0.00, 180.00)
			Main_1.BrickColor = BrickColor.new("Silver flip/flop")
			Main_1.Position = Vector3.new(7.75, 19.75, -4.96)
			Main_1.CFrame = CFrame.new(7.75, 19.75, -4.96, -0.00, -0.00, 1.00)
			Main_1.Parent = __1

			local Arm_1 = Instance.new("Part")
			Arm_1.Name = "Arm"
			Arm_1.TopSurface = Enum.SurfaceType.Smooth
			Arm_1.Color = Color3.new(0.44, 0.43, 0.44)
			Arm_1.Anchored = true
			Arm_1.Size = Vector3.new(1.50, 1.00, 4.00)
			Arm_1.BottomSurface = Enum.SurfaceType.Smooth
			Arm_1.Rotation = Vector3.new(180.00, 0.00, 180.00)
			Arm_1.BrickColor = BrickColor.new("Dark grey")
			Arm_1.Position = Vector3.new(7.75, 21.50, -1.96)
			Arm_1.CFrame = CFrame.new(7.75, 21.50, -1.96, -0.00, -0.00, 1.00)
			Arm_1.Parent = __1

			local Spawner_1 = Instance.new("Part")
			Spawner_1.Name = "Spawner"
			Spawner_1.TopSurface = Enum.SurfaceType.Smooth
			Spawner_1.Color = Color3.new(0.44, 0.43, 0.44)
			Spawner_1.Anchored = true
			Spawner_1.Size = Vector3.new(0.75, 0.50, 0.75)
			Spawner_1.BottomSurface = Enum.SurfaceType.Smooth
			Spawner_1.Rotation = Vector3.new(180.00, 0.00, 180.00)
			Spawner_1.Transparency = 0.25
			Spawner_1.BrickColor = BrickColor.new("Dark grey")
			Spawner_1.Position = Vector3.new(7.75, 20.75, -0.71)
			Spawner_1.CFrame = CFrame.new(7.75, 20.75, -0.71, -0.00, -0.00, 1.00)
			Spawner_1.Parent = __1

			local Dropperscript_1 = Instance.new("Script")
			Dropperscript_1.Name = "Dropperscript"
			Dropperscript_1.Source = "local Dropper\n\nfunction StartDropping()\n	local PlayerName = script.Parent.Parent.Parent.Parent.Claimed.Value\n	local Player = game.Players[PlayerName]\n\n	while task.wait(2) do\n		Dropper.Spawn(Player, script.Parent.Position + Vector3.new(0, -1, 0), script.Parent.Parent.DropAmount.Value)\n	end\nend\n\nrepeat task.wait(1) until script.Parent:IsDescendantOf(workspace)\nDropper = require(game.ServerScriptService:WaitForChild(\'Dropper\'))\nStartDropping()"
			Dropperscript_1.Parent = Spawner_1

			local DropAmount_1 = Instance.new("NumberValue")
			DropAmount_1.Name = "DropAmount"
			DropAmount_1.Value = 2
			DropAmount_1.Parent = __1

			local __1 = Instance.new("Model")
			__1.Name = "5"
			__1.WorldPivot = CFrame.new(7.75, 19.25, -3.00, -0.00, -0.00, 1.00)
			__1.Parent = Upgrades

			local Wall = Instance.new("Part")
			Wall.Name = "Wall"
			Wall.TopSurface = Enum.SurfaceType.Smooth
			Wall.Color = Color3.new(0.53, 0.53, 0.53)
			Wall.Anchored = true
			Wall.Size = Vector3.new(21.00, 2.00, 1.00)
			Wall.BottomSurface = Enum.SurfaceType.Smooth
			Wall.BrickColor = BrickColor.new("Silver flip/flop")
			Wall.Position = Vector3.new(-14.50, 17.00, 24.50)
			Wall.CFrame = CFrame.new(-14.50, 17.00, 24.50, -0.00, -0.00, -1.00)
			Wall.Parent = __1

			local Wall_1 = Instance.new("Part")
			Wall_1.Name = "Wall"
			Wall_1.TopSurface = Enum.SurfaceType.Smooth
			Wall_1.Color = Color3.new(0.53, 0.53, 0.53)
			Wall_1.Anchored = true
			Wall_1.Size = Vector3.new(21.00, 2.00, 1.00)
			Wall_1.BottomSurface = Enum.SurfaceType.Smooth
			Wall_1.BrickColor = BrickColor.new("Silver flip/flop")
			Wall_1.Position = Vector3.new(14.50, 17.00, 24.50)
			Wall_1.CFrame = CFrame.new(14.50, 17.00, 24.50, -0.00, -0.00, -1.00)
			Wall_1.Parent = __1

			local Wall_1 = Instance.new("Part")
			Wall_1.Name = "Wall"
			Wall_1.TopSurface = Enum.SurfaceType.Smooth
			Wall_1.Color = Color3.new(0.53, 0.53, 0.53)
			Wall_1.Anchored = true
			Wall_1.Size = Vector3.new(1.00, 2.00, 49.00)
			Wall_1.BottomSurface = Enum.SurfaceType.Smooth
			Wall_1.BrickColor = BrickColor.new("Silver flip/flop")
			Wall_1.Position = Vector3.new(24.50, 17.00, -0.50)
			Wall_1.CFrame = CFrame.new(24.50, 17.00, -0.50, -0.00, -0.00, -1.00)
			Wall_1.Parent = __1

			local Wall_1 = Instance.new("Part")
			Wall_1.Name = "Wall"
			Wall_1.TopSurface = Enum.SurfaceType.Smooth
			Wall_1.Color = Color3.new(0.53, 0.53, 0.53)
			Wall_1.Anchored = true
			Wall_1.Size = Vector3.new(1.00, 2.00, 49.00)
			Wall_1.BottomSurface = Enum.SurfaceType.Smooth
			Wall_1.BrickColor = BrickColor.new("Silver flip/flop")
			Wall_1.Position = Vector3.new(-24.50, 17.00, -0.50)
			Wall_1.CFrame = CFrame.new(-24.50, 17.00, -0.50, -0.00, -0.00, -1.00)
			Wall_1.Parent = __1

			local Wall_1 = Instance.new("Part")
			Wall_1.Name = "Wall"
			Wall_1.TopSurface = Enum.SurfaceType.Smooth
			Wall_1.Color = Color3.new(0.53, 0.53, 0.53)
			Wall_1.Anchored = true
			Wall_1.Size = Vector3.new(48.00, 2.00, 1.00)
			Wall_1.BottomSurface = Enum.SurfaceType.Smooth
			Wall_1.BrickColor = BrickColor.new("Silver flip/flop")
			Wall_1.Position = Vector3.new(0.00, 17.00, -24.50)
			Wall_1.CFrame = CFrame.new(0.00, 17.00, -24.50, -0.00, -0.00, -1.00)
			Wall_1.Parent = __1

			local __1 = Instance.new("Model")
			__1.Name = "6"
			__1.WorldPivot = CFrame.new(3.00, 16.25, 0.00, -0.00, -0.00, -1.00)
			__1.Parent = Upgrades

			local Wall_1 = Instance.new("Part")
			Wall_1.Name = "Wall"
			Wall_1.TopSurface = Enum.SurfaceType.Smooth
			Wall_1.Color = Color3.new(0.30, 0.30, 0.30)
			Wall_1.Anchored = true
			Wall_1.Size = Vector3.new(28.00, 1.52, 0.50)
			Wall_1.BottomSurface = Enum.SurfaceType.Smooth
			Wall_1.BrickColor = BrickColor.new("Dark taupe")
			Wall_1.Position = Vector3.new(3.00, 16.75, 2.32)
			Wall_1.CFrame = CFrame.new(3.00, 16.75, 2.32, -0.00, -0.00, -1.00)
			Wall_1.Parent = __1

			local Wall_1 = Instance.new("Part")
			Wall_1.Name = "Wall"
			Wall_1.TopSurface = Enum.SurfaceType.Smooth
			Wall_1.Color = Color3.new(0.30, 0.30, 0.30)
			Wall_1.Anchored = true
			Wall_1.Size = Vector3.new(28.00, 1.52, 0.50)
			Wall_1.BottomSurface = Enum.SurfaceType.Smooth
			Wall_1.BrickColor = BrickColor.new("Dark taupe")
			Wall_1.Position = Vector3.new(3.00, 16.75, -2.32)
			Wall_1.CFrame = CFrame.new(3.00, 16.75, -2.32, -0.00, -0.00, -1.00)
			Wall_1.Parent = __1

			local Wall_1 = Instance.new("Part")
			Wall_1.Name = "Wall"
			Wall_1.TopSurface = Enum.SurfaceType.Smooth
			Wall_1.Color = Color3.new(0.30, 0.30, 0.30)
			Wall_1.Anchored = true
			Wall_1.Size = Vector3.new(0.50, 1.52, 5.15)
			Wall_1.BottomSurface = Enum.SurfaceType.Smooth
			Wall_1.BrickColor = BrickColor.new("Dark taupe")
			Wall_1.Position = Vector3.new(-11.25, 16.75, -0.00)
			Wall_1.CFrame = CFrame.new(-11.25, 16.75, -0.00, -0.00, -0.00, -1.00)
			Wall_1.Parent = __1

			local Wall_1 = Instance.new("Part")
			Wall_1.Name = "Wall"
			Wall_1.TopSurface = Enum.SurfaceType.Smooth
			Wall_1.Color = Color3.new(0.30, 0.30, 0.30)
			Wall_1.Anchored = true
			Wall_1.Size = Vector3.new(0.50, 1.52, 5.15)
			Wall_1.BottomSurface = Enum.SurfaceType.Smooth
			Wall_1.BrickColor = BrickColor.new("Dark taupe")
			Wall_1.Position = Vector3.new(17.25, 16.75, -0.00)
			Wall_1.CFrame = CFrame.new(17.25, 16.75, -0.00, -0.00, -0.00, -1.00)
			Wall_1.Parent = __1

			local __1 = Instance.new("Model")
			__1.Name = "7"
			__1.WorldPivot = CFrame.new(3.25, 19.25, -3.21, -0.00, -0.00, 1.00)
			__1.Parent = Upgrades

			local Base_1 = Instance.new("Part")
			Base_1.Name = "Base"
			Base_1.TopSurface = Enum.SurfaceType.Smooth
			Base_1.Color = Color3.new(0.44, 0.43, 0.44)
			Base_1.Anchored = true
			Base_1.Size = Vector3.new(3.00, 1.00, 3.00)
			Base_1.BottomSurface = Enum.SurfaceType.Smooth
			Base_1.Rotation = Vector3.new(180.00, 0.00, 180.00)
			Base_1.BrickColor = BrickColor.new("Dark grey")
			Base_1.Position = Vector3.new(3.25, 16.50, -4.96)
			Base_1.CFrame = CFrame.new(3.25, 16.50, -4.96, -0.00, -0.00, 1.00)
			Base_1.Parent = __1

			local Main_1 = Instance.new("Part")
			Main_1.Name = "Main"
			Main_1.TopSurface = Enum.SurfaceType.Smooth
			Main_1.Color = Color3.new(0.53, 0.52, 0.53)
			Main_1.Anchored = true
			Main_1.Size = Vector3.new(2.00, 5.50, 2.00)
			Main_1.BottomSurface = Enum.SurfaceType.Smooth
			Main_1.Rotation = Vector3.new(180.00, 0.00, 180.00)
			Main_1.BrickColor = BrickColor.new("Silver flip/flop")
			Main_1.Position = Vector3.new(3.25, 19.75, -4.96)
			Main_1.CFrame = CFrame.new(3.25, 19.75, -4.96, -0.00, -0.00, 1.00)
			Main_1.Parent = __1

			local Arm_1 = Instance.new("Part")
			Arm_1.Name = "Arm"
			Arm_1.TopSurface = Enum.SurfaceType.Smooth
			Arm_1.Color = Color3.new(0.44, 0.43, 0.44)
			Arm_1.Anchored = true
			Arm_1.Size = Vector3.new(1.50, 1.00, 4.00)
			Arm_1.BottomSurface = Enum.SurfaceType.Smooth
			Arm_1.Rotation = Vector3.new(180.00, 0.00, 180.00)
			Arm_1.BrickColor = BrickColor.new("Dark grey")
			Arm_1.Position = Vector3.new(3.25, 21.50, -1.96)
			Arm_1.CFrame = CFrame.new(3.25, 21.50, -1.96, -0.00, -0.00, 1.00)
			Arm_1.Parent = __1

			local Spawner_1 = Instance.new("Part")
			Spawner_1.Name = "Spawner"
			Spawner_1.TopSurface = Enum.SurfaceType.Smooth
			Spawner_1.Color = Color3.new(0.44, 0.43, 0.44)
			Spawner_1.Anchored = true
			Spawner_1.Size = Vector3.new(0.75, 0.50, 0.75)
			Spawner_1.BottomSurface = Enum.SurfaceType.Smooth
			Spawner_1.Rotation = Vector3.new(180.00, 0.00, 180.00)
			Spawner_1.Transparency = 0.25
			Spawner_1.BrickColor = BrickColor.new("Dark grey")
			Spawner_1.Position = Vector3.new(3.25, 20.75, -0.71)
			Spawner_1.CFrame = CFrame.new(3.25, 20.75, -0.71, -0.00, -0.00, 1.00)
			Spawner_1.Parent = __1

			local Dropperscript_1 = Instance.new("Script")
			Dropperscript_1.Name = "Dropperscript"
			Dropperscript_1.Source = "local Dropper\n\nfunction StartDropping()\n	local PlayerName = script.Parent.Parent.Parent.Parent.Claimed.Value\n	local Player = game.Players[PlayerName]\n\n	while task.wait(2) do\n		Dropper.Spawn(Player, script.Parent.Position + Vector3.new(0, -1, 0), script.Parent.Parent.DropAmount.Value)\n	end\nend\n\nrepeat task.wait(1) until script.Parent:IsDescendantOf(workspace)\nDropper = require(game.ServerScriptService:WaitForChild(\'Dropper\'))\nStartDropping()"
			Dropperscript_1.Parent = Spawner_1

			local DropAmount_1 = Instance.new("NumberValue")
			DropAmount_1.Name = "DropAmount"
			DropAmount_1.Value = 2
			DropAmount_1.Parent = __1

			local __1 = Instance.new("Model")
			__1.Name = "8"
			__1.WorldPivot = CFrame.new(7.75, 21.25, -3.00, -0.00, -0.00, 1.00)
			__1.Parent = Upgrades

			local Wall_1 = Instance.new("Part")
			Wall_1.Name = "Wall"
			Wall_1.TopSurface = Enum.SurfaceType.Smooth
			Wall_1.Color = Color3.new(0.42, 0.42, 0.42)
			Wall_1.Anchored = true
			Wall_1.Size = Vector3.new(20.90, 2.00, 0.90)
			Wall_1.BottomSurface = Enum.SurfaceType.Smooth
			Wall_1.BrickColor = BrickColor.new("Dark grey")
			Wall_1.Position = Vector3.new(-14.45, 19.00, 24.45)
			Wall_1.CFrame = CFrame.new(-14.45, 19.00, 24.45, -0.00, -0.00, -1.00)
			Wall_1.Parent = __1

			local Wall_1 = Instance.new("Part")
			Wall_1.Name = "Wall"
			Wall_1.TopSurface = Enum.SurfaceType.Smooth
			Wall_1.Color = Color3.new(0.42, 0.42, 0.42)
			Wall_1.Anchored = true
			Wall_1.Size = Vector3.new(20.90, 2.00, 0.90)
			Wall_1.BottomSurface = Enum.SurfaceType.Smooth
			Wall_1.BrickColor = BrickColor.new("Dark grey")
			Wall_1.Position = Vector3.new(14.45, 19.00, 24.45)
			Wall_1.CFrame = CFrame.new(14.45, 19.00, 24.45, -0.00, -0.00, -1.00)
			Wall_1.Parent = __1

			local Wall_1 = Instance.new("Part")
			Wall_1.Name = "Wall"
			Wall_1.TopSurface = Enum.SurfaceType.Smooth
			Wall_1.Color = Color3.new(0.42, 0.42, 0.42)
			Wall_1.Anchored = true
			Wall_1.Size = Vector3.new(0.90, 2.00, 48.90)
			Wall_1.BottomSurface = Enum.SurfaceType.Smooth
			Wall_1.BrickColor = BrickColor.new("Dark grey")
			Wall_1.Position = Vector3.new(24.45, 19.00, -0.45)
			Wall_1.CFrame = CFrame.new(24.45, 19.00, -0.45, -0.00, -0.00, -1.00)
			Wall_1.Parent = __1

			local Wall_1 = Instance.new("Part")
			Wall_1.Name = "Wall"
			Wall_1.TopSurface = Enum.SurfaceType.Smooth
			Wall_1.Color = Color3.new(0.42, 0.42, 0.42)
			Wall_1.Anchored = true
			Wall_1.Size = Vector3.new(0.90, 2.00, 48.90)
			Wall_1.BottomSurface = Enum.SurfaceType.Smooth
			Wall_1.BrickColor = BrickColor.new("Dark grey")
			Wall_1.Position = Vector3.new(-24.45, 19.00, -0.45)
			Wall_1.CFrame = CFrame.new(-24.45, 19.00, -0.45, -0.00, -0.00, -1.00)
			Wall_1.Parent = __1

			local Wall_1 = Instance.new("Part")
			Wall_1.Name = "Wall"
			Wall_1.TopSurface = Enum.SurfaceType.Smooth
			Wall_1.Color = Color3.new(0.42, 0.42, 0.42)
			Wall_1.Anchored = true
			Wall_1.Size = Vector3.new(48.00, 2.00, 0.90)
			Wall_1.BottomSurface = Enum.SurfaceType.Smooth
			Wall_1.BrickColor = BrickColor.new("Dark grey")
			Wall_1.Position = Vector3.new(0.00, 19.00, -24.45)
			Wall_1.CFrame = CFrame.new(0.00, 19.00, -24.45, -0.00, -0.00, -1.00)
			Wall_1.Parent = __1
			local __1 = Instance.new("Model")
			__1.Name = "9"
			__1.WorldPivot = CFrame.new(12.25, 19.25, 3.29, -0.00, -0.00, -1.00)
			__1.Parent = Upgrades

			local Base_1 = Instance.new("Part")
			Base_1.Name = "Base"
			Base_1.TopSurface = Enum.SurfaceType.Smooth
			Base_1.Color = Color3.new(0.44, 0.43, 0.44)
			Base_1.Anchored = true
			Base_1.Size = Vector3.new(3.00, 1.00, 3.00)
			Base_1.BottomSurface = Enum.SurfaceType.Smooth
			Base_1.BrickColor = BrickColor.new("Dark grey")
			Base_1.Position = Vector3.new(12.25, 16.50, 5.04)
			Base_1.CFrame = CFrame.new(12.25, 16.50, 5.04, -0.00, -0.00, -1.00)
			Base_1.Parent = __1

			local Main_1 = Instance.new("Part")
			Main_1.Name = "Main"
			Main_1.TopSurface = Enum.SurfaceType.Smooth
			Main_1.Color = Color3.new(0.53, 0.52, 0.53)
			Main_1.Anchored = true
			Main_1.Size = Vector3.new(2.00, 5.50, 2.00)
			Main_1.BottomSurface = Enum.SurfaceType.Smooth
			Main_1.BrickColor = BrickColor.new("Silver flip/flop")
			Main_1.Position = Vector3.new(12.25, 19.75, 5.04)
			Main_1.CFrame = CFrame.new(12.25, 19.75, 5.04, -0.00, -0.00, -1.00)
			Main_1.Parent = __1

			local Arm_1 = Instance.new("Part")
			Arm_1.Name = "Arm"
			Arm_1.TopSurface = Enum.SurfaceType.Smooth
			Arm_1.Color = Color3.new(0.44, 0.43, 0.44)
			Arm_1.Anchored = true
			Arm_1.Size = Vector3.new(1.50, 1.00, 4.00)
			Arm_1.BottomSurface = Enum.SurfaceType.Smooth
			Arm_1.BrickColor = BrickColor.new("Dark grey")
			Arm_1.Position = Vector3.new(12.25, 21.50, 2.04)
			Arm_1.CFrame = CFrame.new(12.25, 21.50, 2.04, -0.00, -0.00, -1.00)
			Arm_1.Parent = __1

			local Spawner_1 = Instance.new("Part")
			Spawner_1.Name = "Spawner"
			Spawner_1.TopSurface = Enum.SurfaceType.Smooth
			Spawner_1.Color = Color3.new(0.44, 0.43, 0.44)
			Spawner_1.Anchored = true
			Spawner_1.Size = Vector3.new(0.75, 0.50, 0.75)
			Spawner_1.BottomSurface = Enum.SurfaceType.Smooth
			Spawner_1.Transparency = 0.25
			Spawner_1.BrickColor = BrickColor.new("Dark grey")
			Spawner_1.Position = Vector3.new(12.25, 20.75, 0.79)
			Spawner_1.CFrame = CFrame.new(12.25, 20.75, 0.79, -0.00, -0.00, -1.00)
			Spawner_1.Parent = __1

			local Dropperscript_1 = Instance.new("Script")
			Dropperscript_1.Name = "Dropperscript"
			Dropperscript_1.Source = "local Dropper\n\nfunction StartDropping()\n	local PlayerName = script.Parent.Parent.Parent.Parent.Claimed.Value\n	local Player = game.Players[PlayerName]\n\n	while task.wait(2) do\n		Dropper.Spawn(Player, script.Parent.Position + Vector3.new(0, -1, 0), script.Parent.Parent.DropAmount.Value)\n	end\nend\n\nrepeat task.wait(1) until script.Parent:IsDescendantOf(workspace)\nDropper = require(game.ServerScriptService:WaitForChild(\'Dropper\'))\nStartDropping()"
			Dropperscript_1.Parent = Spawner_1

			local DropAmount_1 = Instance.new("NumberValue")
			DropAmount_1.Name = "DropAmount"
			DropAmount_1.Value = 2
			DropAmount_1.Parent = __1

			local _1 = Instance.new("Model")
			_1.Name = "10"
			_1.WorldPivot = CFrame.new(7.75, 23.25, -3.00, -0.00, -0.00, 1.00)
			_1.Parent = Upgrades

			local Wall_1 = Instance.new("Part")
			Wall_1.Name = "Wall"
			Wall_1.TopSurface = Enum.SurfaceType.Smooth
			Wall_1.Color = Color3.new(0.53, 0.53, 0.53)
			Wall_1.Anchored = true
			Wall_1.Size = Vector3.new(21.00, 7.00, 1.00)
			Wall_1.BottomSurface = Enum.SurfaceType.Smooth
			Wall_1.BrickColor = BrickColor.new("Silver flip/flop")
			Wall_1.Position = Vector3.new(-14.50, 23.50, 24.50)
			Wall_1.CFrame = CFrame.new(-14.50, 23.50, 24.50, -0.00, -0.00, -1.00)
			Wall_1.Parent = _1

			local Wall_1 = Instance.new("Part")
			Wall_1.Name = "Wall"
			Wall_1.TopSurface = Enum.SurfaceType.Smooth
			Wall_1.Color = Color3.new(0.53, 0.53, 0.53)
			Wall_1.Anchored = true
			Wall_1.Size = Vector3.new(21.00, 7.00, 1.00)
			Wall_1.BottomSurface = Enum.SurfaceType.Smooth
			Wall_1.BrickColor = BrickColor.new("Silver flip/flop")
			Wall_1.Position = Vector3.new(14.50, 23.50, 24.50)
			Wall_1.CFrame = CFrame.new(14.50, 23.50, 24.50, -0.00, -0.00, -1.00)
			Wall_1.Parent = _1

			local Wall_1 = Instance.new("Part")
			Wall_1.Name = "Wall"
			Wall_1.TopSurface = Enum.SurfaceType.Smooth
			Wall_1.Color = Color3.new(0.53, 0.53, 0.53)
			Wall_1.Anchored = true
			Wall_1.Size = Vector3.new(1.00, 7.00, 49.00)
			Wall_1.BottomSurface = Enum.SurfaceType.Smooth
			Wall_1.BrickColor = BrickColor.new("Silver flip/flop")
			Wall_1.Position = Vector3.new(24.50, 23.50, -0.50)
			Wall_1.CFrame = CFrame.new(24.50, 23.50, -0.50, -0.00, -0.00, -1.00)
			Wall_1.Parent = _1

			local Wall_1 = Instance.new("Part")
			Wall_1.Name = "Wall"
			Wall_1.TopSurface = Enum.SurfaceType.Smooth
			Wall_1.Color = Color3.new(0.53, 0.53, 0.53)
			Wall_1.Anchored = true
			Wall_1.Size = Vector3.new(1.00, 7.00, 49.00)
			Wall_1.BottomSurface = Enum.SurfaceType.Smooth
			Wall_1.BrickColor = BrickColor.new("Silver flip/flop")
			Wall_1.Position = Vector3.new(-24.50, 23.50, -0.50)
			Wall_1.CFrame = CFrame.new(-24.50, 23.50, -0.50, -0.00, -0.00, -1.00)
			Wall_1.Parent = _1

			local Wall_1 = Instance.new("Part")
			Wall_1.Name = "Wall"
			Wall_1.TopSurface = Enum.SurfaceType.Smooth
			Wall_1.Color = Color3.new(0.53, 0.53, 0.53)
			Wall_1.Anchored = true
			Wall_1.Size = Vector3.new(48.00, 7.00, 1.00)
			Wall_1.BottomSurface = Enum.SurfaceType.Smooth
			Wall_1.BrickColor = BrickColor.new("Silver flip/flop")
			Wall_1.Position = Vector3.new(0.00, 23.50, -24.50)
			Wall_1.CFrame = CFrame.new(0.00, 23.50, -24.50, -0.00, -0.00, -1.00)
			Wall_1.Parent = _1

			local Wall_1 = Instance.new("Part")
			Wall_1.Name = "Wall"
			Wall_1.TopSurface = Enum.SurfaceType.Smooth
			Wall_1.Color = Color3.new(0.53, 0.53, 0.53)
			Wall_1.Anchored = true
			Wall_1.Size = Vector3.new(8.00, 3.00, 1.00)
			Wall_1.BottomSurface = Enum.SurfaceType.Smooth
			Wall_1.BrickColor = BrickColor.new("Silver flip/flop")
			Wall_1.Position = Vector3.new(0.00, 25.50, 24.50)
			Wall_1.CFrame = CFrame.new(0.00, 25.50, 24.50, -0.00, -0.00, -1.00)
			Wall_1.Parent = _1

			local _2 = Instance.new("Model")
			_2.Name = "11"
			_2.WorldPivot = CFrame.new(0.00, 15.75, 0.00, -0.00, -0.00, -1.00)
			_2.Parent = Upgrades

			local Ground_1 = Instance.new("Part")
			Ground_1.Name = "Ground"
			Ground_1.TopSurface = Enum.SurfaceType.Smooth
			Ground_1.Color = Color3.new(0.47, 0.32, 0.10)
			Ground_1.Anchored = true
			Ground_1.Material = Enum.Material.SmoothPlastic
			Ground_1.Size = Vector3.new(43.00, 0.50, 48.00)
			Ground_1.BottomSurface = Enum.SurfaceType.Smooth
			Ground_1.BrickColor = BrickColor.new("Rust")
			Ground_1.Position = Vector3.new(2.50, 26.75, 0.00)
			Ground_1.CFrame = CFrame.new(2.50, 26.75, 0.00, -0.00, -0.00, -1.00)
			Ground_1.Parent = _2

			local Texture_1 = Instance.new("Texture")
			Texture_1.Face = Enum.NormalId.Top
			Texture_1.StudsPerTileU = 5
			Texture_1.Transparency = 0.8999999761581421
			Texture_1.StudsPerTileV = 15
			Texture_1.Texture = "rbxassetid://10024137414"
			Texture_1.Parent = Ground_1

			local SurfaceLight = Instance.new("SurfaceLight")
			SurfaceLight.Face = Enum.NormalId.Bottom
			SurfaceLight.Parent = Ground_1

			local Ground_1 = Instance.new("Part")
			Ground_1.Name = "Ground"
			Ground_1.TopSurface = Enum.SurfaceType.Smooth
			Ground_1.Color = Color3.new(0.47, 0.32, 0.10)
			Ground_1.Anchored = true
			Ground_1.Material = Enum.Material.SmoothPlastic
			Ground_1.Size = Vector3.new(5.00, 0.50, 17.00)
			Ground_1.BottomSurface = Enum.SurfaceType.Smooth
			Ground_1.BrickColor = BrickColor.new("Rust")
			Ground_1.Position = Vector3.new(-21.50, 26.75, -15.50)
			Ground_1.CFrame = CFrame.new(-21.50, 26.75, -15.50, -0.00, -0.00, -1.00)
			Ground_1.Parent = _2

			local Texture_1 = Instance.new("Texture")
			Texture_1.Face = Enum.NormalId.Top
			Texture_1.StudsPerTileU = 5
			Texture_1.Transparency = 0.8999999761581421
			Texture_1.StudsPerTileV = 15
			Texture_1.Texture = "rbxassetid://10024137414"
			Texture_1.Parent = Ground_1

			local _3 = Instance.new("Model")
			_3.Name = "12"
			_3.WorldPivot = CFrame.new(0.00, 15.75, 0.00, -0.00, -0.00, -1.00)
			_3.Parent = Upgrades

			local Wood = Instance.new("Part")
			Wood.Name = "Wood"
			Wood.TopSurface = Enum.SurfaceType.Smooth
			Wood.Color = Color3.new(0.47, 0.32, 0.10)
			Wood.Anchored = true
			Wood.Material = Enum.Material.SmoothPlastic
			Wood.Size = Vector3.new(5.00, 0.50, 1.00)
			Wood.BottomSurface = Enum.SurfaceType.Smooth
			Wood.BrickColor = BrickColor.new("Rust")
			Wood.Position = Vector3.new(-21.50, 16.25, 14.50)
			Wood.CFrame = CFrame.new(-21.50, 16.25, 14.50, -0.00, -0.00, -1.00)
			Wood.Parent = _3

			local Texture_1 = Instance.new("Texture")
			Texture_1.Face = Enum.NormalId.Top
			Texture_1.StudsPerTileU = 5
			Texture_1.Transparency = 0.8999999761581421
			Texture_1.StudsPerTileV = 15
			Texture_1.Texture = "rbxassetid://10024137414"
			Texture_1.Parent = Wood

			local Wood_1 = Instance.new("Part")
			Wood_1.Name = "Wood"
			Wood_1.TopSurface = Enum.SurfaceType.Smooth
			Wood_1.Color = Color3.new(0.47, 0.32, 0.10)
			Wood_1.Anchored = true
			Wood_1.Material = Enum.Material.SmoothPlastic
			Wood_1.Size = Vector3.new(5.00, 0.50, 1.00)
			Wood_1.BottomSurface = Enum.SurfaceType.Smooth
			Wood_1.BrickColor = BrickColor.new("Rust")
			Wood_1.Position = Vector3.new(-21.50, 16.75, 13.50)
			Wood_1.CFrame = CFrame.new(-21.50, 16.75, 13.50, -0.00, -0.00, -1.00)
			Wood_1.Parent = _3

			local Texture_1 = Instance.new("Texture")
			Texture_1.Face = Enum.NormalId.Top
			Texture_1.StudsPerTileU = 5
			Texture_1.Transparency = 0.8999999761581421
			Texture_1.StudsPerTileV = 15
			Texture_1.Texture = "rbxassetid://10024137414"
			Texture_1.Parent = Wood_1

			local Wood_1 = Instance.new("Part")
			Wood_1.Name = "Wood"
			Wood_1.TopSurface = Enum.SurfaceType.Smooth
			Wood_1.Color = Color3.new(0.47, 0.32, 0.10)
			Wood_1.Anchored = true
			Wood_1.Material = Enum.Material.SmoothPlastic
			Wood_1.Size = Vector3.new(5.00, 0.50, 1.00)
			Wood_1.BottomSurface = Enum.SurfaceType.Smooth
			Wood_1.BrickColor = BrickColor.new("Rust")
			Wood_1.Position = Vector3.new(-21.50, 17.75, 11.50)
			Wood_1.CFrame = CFrame.new(-21.50, 17.75, 11.50, -0.00, -0.00, -1.00)
			Wood_1.Parent = _3

			local Texture_1 = Instance.new("Texture")
			Texture_1.Face = Enum.NormalId.Top
			Texture_1.StudsPerTileU = 5
			Texture_1.Transparency = 0.8999999761581421
			Texture_1.StudsPerTileV = 15
			Texture_1.Texture = "rbxassetid://10024137414"
			Texture_1.Parent = Wood_1

			local Wood_1 = Instance.new("Part")
			Wood_1.Name = "Wood"
			Wood_1.TopSurface = Enum.SurfaceType.Smooth
			Wood_1.Color = Color3.new(0.47, 0.32, 0.10)
			Wood_1.Anchored = true
			Wood_1.Material = Enum.Material.SmoothPlastic
			Wood_1.Size = Vector3.new(5.00, 0.50, 1.00)
			Wood_1.BottomSurface = Enum.SurfaceType.Smooth
			Wood_1.BrickColor = BrickColor.new("Rust")
			Wood_1.Position = Vector3.new(-21.50, 17.25, 12.50)
			Wood_1.CFrame = CFrame.new(-21.50, 17.25, 12.50, -0.00, -0.00, -1.00)
			Wood_1.Parent = _3

			local Texture_1 = Instance.new("Texture")
			Texture_1.Face = Enum.NormalId.Top
			Texture_1.StudsPerTileU = 5
			Texture_1.Transparency = 0.8999999761581421
			Texture_1.StudsPerTileV = 15
			Texture_1.Texture = "rbxassetid://10024137414"
			Texture_1.Parent = Wood_1

			local Wood_1 = Instance.new("Part")
			Wood_1.Name = "Wood"
			Wood_1.TopSurface = Enum.SurfaceType.Smooth
			Wood_1.Color = Color3.new(0.47, 0.32, 0.10)
			Wood_1.Anchored = true
			Wood_1.Material = Enum.Material.SmoothPlastic
			Wood_1.Size = Vector3.new(5.00, 0.50, 1.00)
			Wood_1.BottomSurface = Enum.SurfaceType.Smooth
			Wood_1.BrickColor = BrickColor.new("Rust")
			Wood_1.Position = Vector3.new(-21.50, 19.75, 7.50)
			Wood_1.CFrame = CFrame.new(-21.50, 19.75, 7.50, -0.00, -0.00, -1.00)
			Wood_1.Parent = _3

			local Texture_1 = Instance.new("Texture")
			Texture_1.Face = Enum.NormalId.Top
			Texture_1.StudsPerTileU = 5
			Texture_1.Transparency = 0.8999999761581421
			Texture_1.StudsPerTileV = 15
			Texture_1.Texture = "rbxassetid://10024137414"
			Texture_1.Parent = Wood_1

			local Wood_1 = Instance.new("Part")
			Wood_1.Name = "Wood"
			Wood_1.TopSurface = Enum.SurfaceType.Smooth
			Wood_1.Color = Color3.new(0.47, 0.32, 0.10)
			Wood_1.Anchored = true
			Wood_1.Material = Enum.Material.SmoothPlastic
			Wood_1.Size = Vector3.new(5.00, 0.50, 1.00)
			Wood_1.BottomSurface = Enum.SurfaceType.Smooth
			Wood_1.BrickColor = BrickColor.new("Rust")
			Wood_1.Position = Vector3.new(-21.50, 19.25, 8.50)
			Wood_1.CFrame = CFrame.new(-21.50, 19.25, 8.50, -0.00, -0.00, -1.00)
			Wood_1.Parent = _3

			local Texture_1 = Instance.new("Texture")
			Texture_1.Face = Enum.NormalId.Top
			Texture_1.StudsPerTileU = 5
			Texture_1.Transparency = 0.8999999761581421
			Texture_1.StudsPerTileV = 15
			Texture_1.Texture = "rbxassetid://10024137414"
			Texture_1.Parent = Wood_1

			local Wood_1 = Instance.new("Part")
			Wood_1.Name = "Wood"
			Wood_1.TopSurface = Enum.SurfaceType.Smooth
			Wood_1.Color = Color3.new(0.47, 0.32, 0.10)
			Wood_1.Anchored = true
			Wood_1.Material = Enum.Material.SmoothPlastic
			Wood_1.Size = Vector3.new(5.00, 0.50, 1.00)
			Wood_1.BottomSurface = Enum.SurfaceType.Smooth
			Wood_1.BrickColor = BrickColor.new("Rust")
			Wood_1.Position = Vector3.new(-21.50, 18.75, 9.50)
			Wood_1.CFrame = CFrame.new(-21.50, 18.75, 9.50, -0.00, -0.00, -1.00)
			Wood_1.Parent = _3

			local Texture_1 = Instance.new("Texture")
			Texture_1.Face = Enum.NormalId.Top
			Texture_1.StudsPerTileU = 5
			Texture_1.Transparency = 0.8999999761581421
			Texture_1.StudsPerTileV = 15
			Texture_1.Texture = "rbxassetid://10024137414"
			Texture_1.Parent = Wood_1

			local Wood_1 = Instance.new("Part")
			Wood_1.Name = "Wood"
			Wood_1.TopSurface = Enum.SurfaceType.Smooth
			Wood_1.Color = Color3.new(0.47, 0.32, 0.10)
			Wood_1.Anchored = true
			Wood_1.Material = Enum.Material.SmoothPlastic
			Wood_1.Size = Vector3.new(5.00, 0.50, 1.00)
			Wood_1.BottomSurface = Enum.SurfaceType.Smooth
			Wood_1.BrickColor = BrickColor.new("Rust")
			Wood_1.Position = Vector3.new(-21.50, 18.25, 10.50)
			Wood_1.CFrame = CFrame.new(-21.50, 18.25, 10.50, -0.00, -0.00, -1.00)
			Wood_1.Parent = _3

			local Texture_1 = Instance.new("Texture")
			Texture_1.Face = Enum.NormalId.Top
			Texture_1.StudsPerTileU = 5
			Texture_1.Transparency = 0.8999999761581421
			Texture_1.StudsPerTileV = 15
			Texture_1.Texture = "rbxassetid://10024137414"
			Texture_1.Parent = Wood_1

			local Wood_1 = Instance.new("Part")
			Wood_1.Name = "Wood"
			Wood_1.TopSurface = Enum.SurfaceType.Smooth
			Wood_1.Color = Color3.new(0.47, 0.32, 0.10)
			Wood_1.Anchored = true
			Wood_1.Material = Enum.Material.SmoothPlastic
			Wood_1.Size = Vector3.new(5.00, 0.50, 1.00)
			Wood_1.BottomSurface = Enum.SurfaceType.Smooth
			Wood_1.BrickColor = BrickColor.new("Rust")
			Wood_1.Position = Vector3.new(-21.50, 20.25, 6.50)
			Wood_1.CFrame = CFrame.new(-21.50, 20.25, 6.50, -0.00, -0.00, -1.00)
			Wood_1.Parent = _3

			local Texture_1 = Instance.new("Texture")
			Texture_1.Face = Enum.NormalId.Top
			Texture_1.StudsPerTileU = 5
			Texture_1.Transparency = 0.8999999761581421
			Texture_1.StudsPerTileV = 15
			Texture_1.Texture = "rbxassetid://10024137414"
			Texture_1.Parent = Wood_1

			local Wood_1 = Instance.new("Part")
			Wood_1.Name = "Wood"
			Wood_1.TopSurface = Enum.SurfaceType.Smooth
			Wood_1.Color = Color3.new(0.47, 0.32, 0.10)
			Wood_1.Anchored = true
			Wood_1.Material = Enum.Material.SmoothPlastic
			Wood_1.Size = Vector3.new(5.00, 0.50, 1.00)
			Wood_1.BottomSurface = Enum.SurfaceType.Smooth
			Wood_1.BrickColor = BrickColor.new("Rust")
			Wood_1.Position = Vector3.new(-21.50, 20.75, 5.50)
			Wood_1.CFrame = CFrame.new(-21.50, 20.75, 5.50, -0.00, -0.00, -1.00)
			Wood_1.Parent = _3

			local Texture_1 = Instance.new("Texture")
			Texture_1.Face = Enum.NormalId.Top
			Texture_1.StudsPerTileU = 5
			Texture_1.Transparency = 0.8999999761581421
			Texture_1.StudsPerTileV = 15
			Texture_1.Texture = "rbxassetid://10024137414"
			Texture_1.Parent = Wood_1
			local Wood_1 = Instance.new("Part")
			Wood_1.Name = "Wood"
			Wood_1.TopSurface = Enum.SurfaceType.Smooth
			Wood_1.Color = Color3.new(0.47, 0.32, 0.10)
			Wood_1.Anchored = true
			Wood_1.Material = Enum.Material.SmoothPlastic
			Wood_1.Size = Vector3.new(5.00, 0.50, 1.00)
			Wood_1.BottomSurface = Enum.SurfaceType.Smooth
			Wood_1.BrickColor = BrickColor.new("Rust")
			Wood_1.Position = Vector3.new(-21.50, 21.75, 3.50)
			Wood_1.CFrame = CFrame.new(-21.50, 21.75, 3.50, -0.00, -0.00, -1.00)
			Wood_1.Parent = _3

			local Texture_1 = Instance.new("Texture")
			Texture_1.Face = Enum.NormalId.Top
			Texture_1.StudsPerTileU = 5
			Texture_1.Transparency = 0.8999999761581421
			Texture_1.StudsPerTileV = 15
			Texture_1.Texture = "rbxassetid://10024137414"
			Texture_1.Parent = Wood_1

			local Wood_1 = Instance.new("Part")
			Wood_1.Name = "Wood"
			Wood_1.TopSurface = Enum.SurfaceType.Smooth
			Wood_1.Color = Color3.new(0.47, 0.32, 0.10)
			Wood_1.Anchored = true
			Wood_1.Material = Enum.Material.SmoothPlastic
			Wood_1.Size = Vector3.new(5.00, 0.50, 1.00)
			Wood_1.BottomSurface = Enum.SurfaceType.Smooth
			Wood_1.BrickColor = BrickColor.new("Rust")
			Wood_1.Position = Vector3.new(-21.50, 21.25, 4.50)
			Wood_1.CFrame = CFrame.new(-21.50, 21.25, 4.50, -0.00, -0.00, -1.00)
			Wood_1.Parent = _3

			local Texture_1 = Instance.new("Texture")
			Texture_1.Face = Enum.NormalId.Top
			Texture_1.StudsPerTileU = 5
			Texture_1.Transparency = 0.8999999761581421
			Texture_1.StudsPerTileV = 15
			Texture_1.Texture = "rbxassetid://10024137414"
			Texture_1.Parent = Wood_1

			local Wood_1 = Instance.new("Part")
			Wood_1.Name = "Wood"
			Wood_1.TopSurface = Enum.SurfaceType.Smooth
			Wood_1.Color = Color3.new(0.47, 0.32, 0.10)
			Wood_1.Anchored = true
			Wood_1.Material = Enum.Material.SmoothPlastic
			Wood_1.Size = Vector3.new(5.00, 0.50, 1.00)
			Wood_1.BottomSurface = Enum.SurfaceType.Smooth
			Wood_1.BrickColor = BrickColor.new("Rust")
			Wood_1.Position = Vector3.new(-21.50, 23.25, 0.50)
			Wood_1.CFrame = CFrame.new(-21.50, 23.25, 0.50, -0.00, -0.00, -1.00)
			Wood_1.Parent = _3

			local Texture_1 = Instance.new("Texture")
			Texture_1.Face = Enum.NormalId.Top
			Texture_1.StudsPerTileU = 5
			Texture_1.Transparency = 0.8999999761581421
			Texture_1.StudsPerTileV = 15
			Texture_1.Texture = "rbxassetid://10024137414"
			Texture_1.Parent = Wood_1

			local Wood_1 = Instance.new("Part")
			Wood_1.Name = "Wood"
			Wood_1.TopSurface = Enum.SurfaceType.Smooth
			Wood_1.Color = Color3.new(0.47, 0.32, 0.10)
			Wood_1.Anchored = true
			Wood_1.Material = Enum.Material.SmoothPlastic
			Wood_1.Size = Vector3.new(5.00, 0.50, 1.00)
			Wood_1.BottomSurface = Enum.SurfaceType.Smooth
			Wood_1.BrickColor = BrickColor.new("Rust")
			Wood_1.Position = Vector3.new(-21.50, 23.75, -0.50)
			Wood_1.CFrame = CFrame.new(-21.50, 23.75, -0.50, -0.00, -0.00, -1.00)
			Wood_1.Parent = _3

			local Texture_1 = Instance.new("Texture")
			Texture_1.Face = Enum.NormalId.Top
			Texture_1.StudsPerTileU = 5
			Texture_1.Transparency = 0.8999999761581421
			Texture_1.StudsPerTileV = 15
			Texture_1.Texture = "rbxassetid://10024137414"
			Texture_1.Parent = Wood_1

			local Wood_1 = Instance.new("Part")
			Wood_1.Name = "Wood"
			Wood_1.TopSurface = Enum.SurfaceType.Smooth
			Wood_1.Color = Color3.new(0.47, 0.32, 0.10)
			Wood_1.Anchored = true
			Wood_1.Material = Enum.Material.SmoothPlastic
			Wood_1.Size = Vector3.new(5.00, 0.50, 1.00)
			Wood_1.BottomSurface = Enum.SurfaceType.Smooth
			Wood_1.BrickColor = BrickColor.new("Rust")
			Wood_1.Position = Vector3.new(-21.50, 22.75, 1.50)
			Wood_1.CFrame = CFrame.new(-21.50, 22.75, 1.50, -0.00, -0.00, -1.00)
			Wood_1.Parent = _3

			local Texture_1 = Instance.new("Texture")
			Texture_1.Face = Enum.NormalId.Top
			Texture_1.StudsPerTileU = 5
			Texture_1.Transparency = 0.8999999761581421
			Texture_1.StudsPerTileV = 15
			Texture_1.Texture = "rbxassetid://10024137414"
			Texture_1.Parent = Wood_1

			local Wood_1 = Instance.new("Part")
			Wood_1.Name = "Wood"
			Wood_1.TopSurface = Enum.SurfaceType.Smooth
			Wood_1.Color = Color3.new(0.47, 0.32, 0.10)
			Wood_1.Anchored = true
			Wood_1.Material = Enum.Material.SmoothPlastic
			Wood_1.Size = Vector3.new(5.00, 0.50, 1.00)
			Wood_1.BottomSurface = Enum.SurfaceType.Smooth
			Wood_1.BrickColor = BrickColor.new("Rust")
			Wood_1.Position = Vector3.new(-21.50, 22.25, 2.50)
			Wood_1.CFrame = CFrame.new(-21.50, 22.25, 2.50, -0.00, -0.00, -1.00)
			Wood_1.Parent = _3

			local Texture_1 = Instance.new("Texture")
			Texture_1.Face = Enum.NormalId.Top
			Texture_1.StudsPerTileU = 5
			Texture_1.Transparency = 0.8999999761581421
			Texture_1.StudsPerTileV = 15
			Texture_1.Texture = "rbxassetid://10024137414"
			Texture_1.Parent = Wood_1

			local Wood_1 = Instance.new("Part")
			Wood_1.Name = "Wood"
			Wood_1.TopSurface = Enum.SurfaceType.Smooth
			Wood_1.Color = Color3.new(0.47, 0.32, 0.10)
			Wood_1.Anchored = true
			Wood_1.Material = Enum.Material.SmoothPlastic
			Wood_1.Size = Vector3.new(5.00, 0.50, 1.00)
			Wood_1.BottomSurface = Enum.SurfaceType.Smooth
			Wood_1.BrickColor = BrickColor.new("Rust")
			Wood_1.Position = Vector3.new(-21.50, 24.75, -2.50)
			Wood_1.CFrame = CFrame.new(-21.50, 24.75, -2.50, -0.00, -0.00, -1.00)
			Wood_1.Parent = _3

			local Texture_1 = Instance.new("Texture")
			Texture_1.Face = Enum.NormalId.Top
			Texture_1.StudsPerTileU = 5
			Texture_1.Transparency = 0.8999999761581421
			Texture_1.StudsPerTileV = 15
			Texture_1.Texture = "rbxassetid://10024137414"
			Texture_1.Parent = Wood_1

			local Wood_1 = Instance.new("Part")
			Wood_1.Name = "Wood"
			Wood_1.TopSurface = Enum.SurfaceType.Smooth
			Wood_1.Color = Color3.new(0.47, 0.32, 0.10)
			Wood_1.Anchored = true
			Wood_1.Material = Enum.Material.SmoothPlastic
			Wood_1.Size = Vector3.new(5.00, 0.50, 1.00)
			Wood_1.BottomSurface = Enum.SurfaceType.Smooth
			Wood_1.BrickColor = BrickColor.new("Rust")
			Wood_1.Position = Vector3.new(-21.50, 24.25, -1.50)
			Wood_1.CFrame = CFrame.new(-21.50, 24.25, -1.50, -0.00, -0.00, -1.00)
			Wood_1.Parent = _3

			local Texture_1 = Instance.new("Texture")
			Texture_1.Face = Enum.NormalId.Top
			Texture_1.StudsPerTileU = 5
			Texture_1.Transparency = 0.8999999761581421
			Texture_1.StudsPerTileV = 15
			Texture_1.Texture = "rbxassetid://10024137414"
			Texture_1.Parent = Wood_1

			local Wood_1 = Instance.new("Part")
			Wood_1.Name = "Wood"
			Wood_1.TopSurface = Enum.SurfaceType.Smooth
			Wood_1.Color = Color3.new(0.47, 0.32, 0.10)
			Wood_1.Anchored = true
			Wood_1.Material = Enum.Material.SmoothPlastic
			Wood_1.Size = Vector3.new(5.00, 0.50, 1.00)
			Wood_1.BottomSurface = Enum.SurfaceType.Smooth
			Wood_1.BrickColor = BrickColor.new("Rust")
			Wood_1.Position = Vector3.new(-21.50, 25.25, -3.50)
			Wood_1.CFrame = CFrame.new(-21.50, 25.25, -3.50, -0.00, -0.00, -1.00)
			Wood_1.Parent = _3

			local Texture_1 = Instance.new("Texture")
			Texture_1.Face = Enum.NormalId.Top
			Texture_1.StudsPerTileU = 5
			Texture_1.Transparency = 0.8999999761581421
			Texture_1.StudsPerTileV = 15
			Texture_1.Texture = "rbxassetid://10024137414"
			Texture_1.Parent = Wood_1

			local Wood_1 = Instance.new("Part")
			Wood_1.Name = "Wood"
			Wood_1.TopSurface = Enum.SurfaceType.Smooth
			Wood_1.Color = Color3.new(0.47, 0.32, 0.10)
			Wood_1.Anchored = true
			Wood_1.Material = Enum.Material.SmoothPlastic
			Wood_1.Size = Vector3.new(5.00, 0.50, 1.00)
			Wood_1.BottomSurface = Enum.SurfaceType.Smooth
			Wood_1.BrickColor = BrickColor.new("Rust")
			Wood_1.Position = Vector3.new(-21.50, 25.75, -4.50)
			Wood_1.CFrame = CFrame.new(-21.50, 25.75, -4.50, -0.00, -0.00, -1.00)
			Wood_1.Parent = _3

			local Texture_1 = Instance.new("Texture")
			Texture_1.Face = Enum.NormalId.Top
			Texture_1.StudsPerTileU = 5
			Texture_1.Transparency = 0.8999999761581421
			Texture_1.StudsPerTileV = 15
			Texture_1.Texture = "rbxassetid://10024137414"
			Texture_1.Parent = Wood_1

			local Wood_1 = Instance.new("Part")
			Wood_1.Name = "Wood"
			Wood_1.TopSurface = Enum.SurfaceType.Smooth
			Wood_1.Color = Color3.new(0.47, 0.32, 0.10)
			Wood_1.Anchored = true
			Wood_1.Material = Enum.Material.SmoothPlastic
			Wood_1.Size = Vector3.new(5.00, 0.50, 1.00)
			Wood_1.BottomSurface = Enum.SurfaceType.Smooth
			Wood_1.BrickColor = BrickColor.new("Rust")
			Wood_1.Position = Vector3.new(-21.50, 26.75, -6.50)
			Wood_1.CFrame = CFrame.new(-21.50, 26.75, -6.50, -0.00, -0.00, -1.00)
			Wood_1.Parent = _3

			local Texture_1 = Instance.new("Texture")
			Texture_1.Face = Enum.NormalId.Top
			Texture_1.StudsPerTileU = 5
			Texture_1.Transparency = 0.8999999761581421
			Texture_1.StudsPerTileV = 15
			Texture_1.Texture = "rbxassetid://10024137414"
			Texture_1.Parent = Wood_1

			local Wood_1 = Instance.new("Part")
			Wood_1.Name = "Wood"
			Wood_1.TopSurface = Enum.SurfaceType.Smooth
			Wood_1.Color = Color3.new(0.47, 0.32, 0.10)
			Wood_1.Anchored = true
			Wood_1.Material = Enum.Material.SmoothPlastic
			Wood_1.Size = Vector3.new(5.00, 0.50, 1.00)
			Wood_1.BottomSurface = Enum.SurfaceType.Smooth
			Wood_1.BrickColor = BrickColor.new("Rust")
			Wood_1.Position = Vector3.new(-21.50, 26.25, -5.50)
			Wood_1.CFrame = CFrame.new(-21.50, 26.25, -5.50, -0.00, -0.00, -1.00)
			Wood_1.Parent = _3

			local Texture_1 = Instance.new("Texture")
			Texture_1.Face = Enum.NormalId.Top
			Texture_1.StudsPerTileU = 5
			Texture_1.Transparency = 0.8999999761581421
			Texture_1.StudsPerTileV = 15
			Texture_1.Texture = "rbxassetid://10024137414"
			Texture_1.Parent = Wood_1

			local _4 = Instance.new("Model")
			_4.Name = "13"
			_4.WorldPivot = CFrame.new(0.00, 19.50, 24.50, -0.00, -0.00, -1.00)
			_4.Parent = Upgrades

			local Killpart = Instance.new("Part")
			Killpart.Name = "Killpart"
			Killpart.TopSurface = Enum.SurfaceType.Smooth
			Killpart.Color = Color3.new(0.21, 0.21, 0.21)
			Killpart.Anchored = true
			Killpart.Size = Vector3.new(6.00, 7.00, 1.00)
			Killpart.BottomSurface = Enum.SurfaceType.Smooth
			Killpart.CanCollide = false
			Killpart.Transparency = 1
			Killpart.BrickColor = BrickColor.new("Black")
			Killpart.Position = Vector3.new(0.00, 19.50, 24.50)
			Killpart.CFrame = CFrame.new(0.00, 19.50, 24.50, -0.00, -0.00, -1.00)
			Killpart.Parent = _4

			local Laser = Instance.new("Part")
			Laser.Name = "Laser"
			Laser.TopSurface = Enum.SurfaceType.Smooth
			Laser.Color = Color3.new(1.00, 0.00, 0.00)
			Laser.Anchored = true
			Laser.Material = Enum.Material.Neon
			Laser.Size = Vector3.new(6.00, 0.75, 0.75)
			Laser.BottomSurface = Enum.SurfaceType.Smooth
			Laser.CanCollide = false
			Laser.BrickColor = BrickColor.new("Really red")
			Laser.Position = Vector3.new(0.00, 18.25, 24.50)
			Laser.CFrame = CFrame.new(0.00, 18.25, 24.50, -0.00, -0.00, -1.00)
			Laser.Parent = _4

			local Laser_1 = Instance.new("Part")
			Laser_1.Name = "Laser"
			Laser_1.TopSurface = Enum.SurfaceType.Smooth
			Laser_1.Color = Color3.new(1.00, 0.00, 0.00)
			Laser_1.Anchored = true
			Laser_1.Material = Enum.Material.Neon
			Laser_1.Size = Vector3.new(6.00, 0.75, 0.75)
			Laser_1.BottomSurface = Enum.SurfaceType.Smooth
			Laser_1.CanCollide = false
			Laser_1.BrickColor = BrickColor.new("Really red")
			Laser_1.Position = Vector3.new(0.00, 16.75, 24.50)
			Laser_1.CFrame = CFrame.new(0.00, 16.75, 24.50, -0.00, -0.00, -1.00)
			Laser_1.Parent = _4

			local Laser_1 = Instance.new("Part")
			Laser_1.Name = "Laser"
			Laser_1.TopSurface = Enum.SurfaceType.Smooth
			Laser_1.Color = Color3.new(1.00, 0.00, 0.00)
			Laser_1.Anchored = true
			Laser_1.Material = Enum.Material.Neon
			Laser_1.Size = Vector3.new(6.00, 0.75, 0.75)
			Laser_1.BottomSurface = Enum.SurfaceType.Smooth
			Laser_1.CanCollide = false
			Laser_1.BrickColor = BrickColor.new("Really red")
			Laser_1.Position = Vector3.new(0.00, 21.25, 24.50)
			Laser_1.CFrame = CFrame.new(0.00, 21.25, 24.50, -0.00, -0.00, -1.00)
			Laser_1.Parent = _4

			local Laser_1 = Instance.new("Part")
			Laser_1.Name = "Laser"
			Laser_1.TopSurface = Enum.SurfaceType.Smooth
			Laser_1.Color = Color3.new(1.00, 0.00, 0.00)
			Laser_1.Anchored = true
			Laser_1.Material = Enum.Material.Neon
			Laser_1.Size = Vector3.new(6.00, 0.75, 0.75)
			Laser_1.BottomSurface = Enum.SurfaceType.Smooth
			Laser_1.CanCollide = false
			Laser_1.BrickColor = BrickColor.new("Really red")
			Laser_1.Position = Vector3.new(0.00, 19.75, 24.50)
			Laser_1.CFrame = CFrame.new(0.00, 19.75, 24.50, -0.00, -0.00, -1.00)
			Laser_1.Parent = _4

			local Laser_1 = Instance.new("Part")
			Laser_1.Name = "Laser"
			Laser_1.TopSurface = Enum.SurfaceType.Smooth
			Laser_1.Color = Color3.new(1.00, 0.00, 0.00)
			Laser_1.Anchored = true
			Laser_1.Material = Enum.Material.Neon
			Laser_1.Size = Vector3.new(6.00, 0.75, 0.75)
			Laser_1.BottomSurface = Enum.SurfaceType.Smooth
			Laser_1.CanCollide = false
			Laser_1.BrickColor = BrickColor.new("Really red")
			Laser_1.Position = Vector3.new(0.00, 22.62, 24.50)
			Laser_1.CFrame = CFrame.new(0.00, 22.62, 24.50, -0.00, -0.00, -1.00)
			Laser_1.Parent = _4

			local KillHandler = Instance.new("Script")
			KillHandler.Name = "KillHandler"
			KillHandler.Source = "--// Variables\nlocal Killpart = script.Parent.Killpart\nlocal Owner = script.Parent.Parent.Parent.Claimed\n\n--// Functions\nlocal function OnTouched(Hit)\n	local Character = Hit.Parent\n	if not Hit.Parent:FindFirstChild(\'Humanoid\') then return end -- Not a player\n	\n	if Character.Name == Owner.Value then return end -- Player is the owner\n	\n	Character.Health = 0\nend\n\n--// Connections\nKillpart.Touched:Connect(OnTouched)"
			KillHandler.Parent = _4

			local _5 = Instance.new("Model")
			_5.Name = "14"
			_5.WorldPivot = CFrame.new(-6.20, 17.26, -0.00, -0.02, -0.00, 1.00)
			_5.Parent = Upgrades

			local Upgrader = Instance.new("MeshPart")
			Upgrader.Name = "Upgrader"
			Upgrader.Anchored = true
			Upgrader.RenderFidelity = Enum.RenderFidelity.Automatic
			Upgrader.CanCollide = false
			Upgrader.MeshId = "rbxassetid://14089249693"
			Upgrader.Transparency = 0.25
			Upgrader.DoubleSided = true
			Upgrader.CanQuery = false
			Upgrader.Color = Color3.new(1.00, 0.00, 0.00)
			Upgrader.Material = Enum.Material.Neon
			Upgrader.Size = Vector3.new(0.16, 1.50, 4.15)
			Upgrader.Rotation = Vector3.new(180.00, 0.93, 0.00)
			Upgrader.BrickColor = BrickColor.new("Really red")
			Upgrader.Position = Vector3.new(-6.20, 17.26, -0.00)
			Upgrader.CFrame = CFrame.new(-6.20, 17.26, -0.00, -0.02, -0.00, 1.00)
			Upgrader.CastShadow = false
			Upgrader.Parent = _5

			local Script = Instance.new("Script")
			Script.Source = "-- Made by GalazySide, Edited by LucaDaBoy\n\nlocal Upgrader = script.Parent\nlocal Multiplier = Upgrader.Multiplier.Value\n\nlocal PartsUpgraded = {}\n\nlocal function onTouched(hit)\n	if not hit:IsDescendantOf(workspace.DropperParts) then return end\n	if PartsUpgraded[hit] then return end\n	\n	hit.Worth.Value *= Multiplier\n	\n	-- So it's only upgraded once, one collision\n	PartsUpgraded[hit] = true\n	task.wait(10)\n	PartsUpgraded[hit] = nil\nend\n\n-- Connect the Touched event to the function\nUpgrader.Touched:Connect(onTouched)"
			Script.Parent = Upgrader

			local Multiplier = Instance.new("NumberValue")
			Multiplier.Name = "Multiplier"
			Multiplier.Value = 2
			Multiplier.Parent = Upgrader

			local RobuxButtons = Instance.new("Folder")
			RobuxButtons.Name = "RobuxButtons"
			RobuxButtons.Parent = TemplatePlot

			local __1 = Instance.new("Part")
			__1.Name = "1"
			__1.TopSurface = Enum.SurfaceType.Smooth
			__1.Color = Color3.new(0.33, 1.00, 0.00)
			__1.Shape = Enum.PartType.Cylinder
			__1.Anchored = true
			__1.Size = Vector3.new(0.50, 3.50, 3.50)
			__1.BottomSurface = Enum.SurfaceType.Smooth
			__1.Rotation = Vector3.new(-90.00, 90.00, 0.00)
			__1.BrickColor = BrickColor.new("Lime green")
			__1.Position = Vector3.new(-8.50, 16.25, 5.79)
			__1.CFrame = CFrame.new(-8.50, 16.25, 5.79, -1.00, -0.00, -0.00)
			__1.Parent = RobuxButtons
			local BillboardGui_1 = Instance.new("BillboardGui")
			BillboardGui_1.Active = true
			BillboardGui_1.Size = UDim2.new(4.00, 0.00, 1.00, 0.00)
			BillboardGui_1.ClipsDescendants = true
			BillboardGui_1.MaxDistance = 100
			BillboardGui_1.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
			BillboardGui_1.StudsOffset = Vector3.new(0.00, 1.50, 0.00)
			BillboardGui_1.Parent = __1

			local Price_1 = Instance.new("TextLabel")
			Price_1.Name = "Price"
			Price_1.TextWrapped = true
			Price_1.BorderSizePixel = 0
			Price_1.TextScaled = true
			Price_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Price_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Price_1.TextSize = 14
			Price_1.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Price_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Price_1.Text = "19 Robux"
			Price_1.TextColor3 = Color3.new(0.47, 1.00, 0.24)
			Price_1.BackgroundTransparency = 1
			Price_1.Position = UDim2.new(0.00, 0.00, 0.50, 0.00)
			Price_1.Parent = BillboardGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Price_1

			local Item_1 = Instance.new("TextLabel")
			Item_1.Name = "Item"
			Item_1.TextWrapped = true
			Item_1.BorderSizePixel = 0
			Item_1.TextScaled = true
			Item_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Item_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Item_1.TextSize = 14
			Item_1.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Item_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Item_1.Text = "+1,000$"
			Item_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Item_1.BackgroundTransparency = 1
			Item_1.Parent = BillboardGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Item_1

			local ProductId = Instance.new("IntValue")
			ProductId.Name = "ProductId"
			ProductId.Value = 1881648985
			ProductId.Parent = __1

			local Amount = Instance.new("NumberValue")
			Amount.Name = "Amount"
			Amount.Value = 1000
			Amount.Parent = __1

			local __1 = Instance.new("Part")
			__1.Name = "2"
			__1.TopSurface = Enum.SurfaceType.Smooth
			__1.Color = Color3.new(0.33, 1.00, 0.00)
			__1.Shape = Enum.PartType.Cylinder
			__1.Anchored = true
			__1.Size = Vector3.new(0.50, 3.50, 3.50)
			__1.BottomSurface = Enum.SurfaceType.Smooth
			__1.Rotation = Vector3.new(-90.00, 90.00, 0.00)
			__1.BrickColor = BrickColor.new("Lime green")
			__1.Position = Vector3.new(-4.50, 16.25, 5.79)
			__1.CFrame = CFrame.new(-4.50, 16.25, 5.79, -1.00, -0.00, -0.00)
			__1.Parent = RobuxButtons

			local BillboardGui_1 = Instance.new("BillboardGui")
			BillboardGui_1.Active = true
			BillboardGui_1.Size = UDim2.new(4.00, 0.00, 1.00, 0.00)
			BillboardGui_1.ClipsDescendants = true
			BillboardGui_1.MaxDistance = 100
			BillboardGui_1.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
			BillboardGui_1.StudsOffset = Vector3.new(0.00, 1.50, 0.00)
			BillboardGui_1.Parent = __1

			local Price_1 = Instance.new("TextLabel")
			Price_1.Name = "Price"
			Price_1.TextWrapped = true
			Price_1.BorderSizePixel = 0
			Price_1.TextScaled = true
			Price_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Price_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Price_1.TextSize = 14
			Price_1.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Price_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Price_1.Text = "49 Robux"
			Price_1.TextColor3 = Color3.new(0.47, 1.00, 0.24)
			Price_1.BackgroundTransparency = 1
			Price_1.Position = UDim2.new(0.00, 0.00, 0.50, 0.00)
			Price_1.Parent = BillboardGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Price_1

			local Item_1 = Instance.new("TextLabel")
			Item_1.Name = "Item"
			Item_1.TextWrapped = true
			Item_1.BorderSizePixel = 0
			Item_1.TextScaled = true
			Item_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Item_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Item_1.TextSize = 14
			Item_1.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Item_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Item_1.Text = "+10,000$"
			Item_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Item_1.BackgroundTransparency = 1
			Item_1.Parent = BillboardGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Item_1

			local ProductId_1 = Instance.new("IntValue")
			ProductId_1.Name = "ProductId"
			ProductId_1.Value = 1881649846
			ProductId_1.Parent = __1

			local Amount_1 = Instance.new("NumberValue")
			Amount_1.Name = "Amount"
			Amount_1.Value = 10000
			Amount_1.Parent = __1

			local __1 = Instance.new("Part")
			__1.Name = "3"
			__1.TopSurface = Enum.SurfaceType.Smooth
			__1.Color = Color3.new(0.33, 1.00, 0.00)
			__1.Shape = Enum.PartType.Cylinder
			__1.Anchored = true
			__1.Size = Vector3.new(0.50, 3.50, 3.50)
			__1.BottomSurface = Enum.SurfaceType.Smooth
			__1.Rotation = Vector3.new(-90.00, 90.00, 0.00)
			__1.BrickColor = BrickColor.new("Lime green")
			__1.Position = Vector3.new(-0.50, 16.25, 5.79)
			__1.CFrame = CFrame.new(-0.50, 16.25, 5.79, -1.00, -0.00, -0.00)
			__1.Parent = RobuxButtons

			local BillboardGui_1 = Instance.new("BillboardGui")
			BillboardGui_1.Active = true
			BillboardGui_1.Size = UDim2.new(4.00, 0.00, 1.00, 0.00)
			BillboardGui_1.ClipsDescendants = true
			BillboardGui_1.MaxDistance = 100
			BillboardGui_1.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
			BillboardGui_1.StudsOffset = Vector3.new(0.00, 1.50, 0.00)
			BillboardGui_1.Parent = __1

			local Price_1 = Instance.new("TextLabel")
			Price_1.Name = "Price"
			Price_1.TextWrapped = true
			Price_1.BorderSizePixel = 0
			Price_1.TextScaled = true
			Price_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Price_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Price_1.TextSize = 14
			Price_1.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Price_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Price_1.Text = "99 Robux"
			Price_1.TextColor3 = Color3.new(0.47, 1.00, 0.24)
			Price_1.BackgroundTransparency = 1
			Price_1.Position = UDim2.new(0.00, 0.00, 0.50, 0.00)
			Price_1.Parent = BillboardGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Price_1

			local Item_1 = Instance.new("TextLabel")
			Item_1.Name = "Item"
			Item_1.TextWrapped = true
			Item_1.BorderSizePixel = 0
			Item_1.TextScaled = true
			Item_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Item_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Item_1.TextSize = 14
			Item_1.Size = UDim2.new(1.00, 0.00, 0.50, 0.00)
			Item_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Item_1.Text = "+100,000$"
			Item_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Item_1.BackgroundTransparency = 1
			Item_1.Parent = BillboardGui_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Item_1

			local ProductId_1 = Instance.new("IntValue")
			ProductId_1.Name = "ProductId"
			ProductId_1.Value = 1881650038
			ProductId_1.Parent = __1

			local Amount_1 = Instance.new("NumberValue")
			Amount_1.Name = "Amount"
			Amount_1.Value = 100000
			Amount_1.Parent = __1


			--REPLICATED STORAGE (MODULE SCRIPTS) "MULTIPLIERS"
			-- In this module you can edit the multiplier's in game.

			local Multipliers = {}

			--// Services
			local ReplicatedStorage = game:GetService("ReplicatedStorage")

			--// Imports
			local Stat = require(ReplicatedStorage.Stat)

			--// Main
			function Multipliers.GetMoneyMultiplier(Player)
				local Multi = 1

				-- Gamepass
				local DoubleMoneyExists = ReplicatedStorage.GamepassIds:FindFirstChild("DoubleMoney")

				if DoubleMoneyExists then
					local DoubleMoneyOwned = Stat.Get(Player, "DoubleMoney").Value

					if DoubleMoneyOwned then
						Multi *= 2
					end
				end

				-- Rebirth
				local Rebirth = Stat.Get(Player, "Rebirth")
				Multi *= (Rebirth.Value + 1)

				return Multi	
			end

			return Multipliers
			
			
			

			--REPLICATED STORAGE (MODULE SCRIPTS) "SHORT"
			-- i will one day optimize this module

			local Module = {}

			Module.Prefixes = {"K","M","B","T","Qd","Qn","Sx","Sp","Oc","No",
				"De","UDe","DDe","TDe","QtDe","QnDe","SxDe","SpDe","OcDe","NoDe",
				"Vg","UVg","DVg","TVg","QdVg","QnVg","SxVg","SpVg","OcVg","NoVg",
				"Tg","UTg","DTg","TTg","QdTg","QnTg","SxTg","SpTg","OcTg","NoTg",
				"qg","Uqg","Dqg","Tqg","Qdqg","Qnqg","Sxqg","Spqg","Ocqg","Noqg",
				"Qg","UQg","DQg","TQg","QdQg","QnQg","SxQg","SpQg","OcQg","NoQg",
				"sg","Usg","Dsg","Tsg","Qdsg","Qnsg","Sxsg","Spsg","Ocsg","Nosg",
				"Sg","USg","DSg","TSg","QdSg","QnSg","SxSg","SpSg","OcSg","NoSg",
				"Og","UOg","DOg","TOg","QdOg","QnOg","SxOg","SpOg","OcOg","NoOg",
				"Ng","UNg","DNg","TNg","QdNg","QnNg","SxNg","SpNg","OcNg","NoNg",
				"Ce"}


			function Module.CutDigits(x)
				if x - math.floor(x) == 0 then return x end
				return string.format("%.2f", x)
			end


			function Module.toSuffix(number, digits)
				if number == 0 then return number end
				if number < 1 then return Module.CutDigits(number) end

				number = (number < 0 and math.abs(number)) or number
				digits = digits or 2

				local suffix = math.floor(math.log10(number)/3)

				return Module.CutDigits(number / 1000^(suffix)) .. ( Module.Prefixes[math.floor(suffix)] or "")
			end

			function Module.toTime(val)
				if not tonumber(val) then return val end

				local days = math.floor(val / 86400)
				val = val - days * 86400

				local hours = math.floor(val / 3600)
				val = val - hours * 3600

				local mins = math.floor(val / 60)
				val = val - mins * 60

				val = val > 0 and " " .. math.floor(val) .. "s" or ""
				return (days > 0 and days .. "d" or "") .. (hours > 0 and " " .. hours .. "h" or "") .. (mins > 0 and " " .. mins .. "m" or "") .. val
			end

			function Module.toDate(val)
				if not tonumber(val) then return val end

				local DateTable = os.date("!*t", val)
				local Months = {"Jan","Feb","Mar","Apr","May","Jun","Jul","Aug","Sep","Oct","Nov","Dec"}

				return DateTable.day.." "..Months[DateTable.month].." "..DateTable.year
			end

			return Module
			
			--REPLICATED STORAGE (MODULE SCRIPTS) "STAT"
	--[[
	HOW TO USE THIS MODULE
	
	Stat.Get(Player, StatName(string)) returns the Stat instance, looks through all folders in ReplicatedStorage.Data until it's found.
	Stat.GetDataFolder(Player) returns ReplicatedStorage.Data[PlayerName]
	Stat.WaitForLoad(Player) loads and returns a boolean wether the loading succeeded or not.
	
	]]

			local Stat = {}
			Stat.Cached = {} -- Stat's that have been looked up previously are stored here. This makes it so there's no searching the 2nd time you use it

			local Data

			local function CreatePath(EndInstance, StartInstance)
				local Path = {}
				local CurrentLayer = StartInstance
				repeat -- loop that imports the names of the parents
					table.insert(Path, 1, CurrentLayer.Parent.Name)
					CurrentLayer = CurrentLayer.Parent
				until -- until the parent is the playerdata
				CurrentLayer.Parent == EndInstance
				return Path
			end

			local function ReadPath(Path, StartInstance)
				local StatInstance = StartInstance
				for _, Child in Path do
					StatInstance = StatInstance[Child] -- this creates the path one by one
				end
				return StatInstance
			end

			function Stat.Get(Player: Player, StatName: string) -- returns stat instance
				if StatName == nil then -- the Player argument is actually the StatName, and StatName is nil, aka its called from the client
					StatName = Player
					Player = game.Players.LocalPlayer
				end

				if not Data then
					Data = game.ReplicatedStorage:WaitForChild("Data")
				end

				local PlayerData = Data:FindFirstChild(Player.Name)

				if not PlayerData then
					task.wait(0.1)
					return Stat.Get(Player, StatName)
				end

				local CachedStat = Stat.Cached[StatName]
				if CachedStat then -- stat is being looked up for the second time if this is true
					return CachedStat == {} and PlayerData[StatName] or ReadPath(CachedStat, PlayerData)[StatName] -- returns a StatInstance
				end

				-- first time u look up the stat
				if PlayerData.Stats:FindFirstChild(StatName) then
					Stat.Cached[StatName] = {"Stats"}
					return PlayerData.Stats[StatName]
				else
					for _,v in PlayerData:GetDescendants() do
						if v.Name == StatName then
							Stat.Cached[StatName] = {}

							--// Creates a path and puts it into the Cached folder so it can be accessed directly next time the stat is looked up
							if v.Parent ~= PlayerData then -- check if it even has a path
								Stat.Cached[StatName] = CreatePath(PlayerData, v) -- creates a table with the childnames to create the path
							end

							return v
						end
					end
				end

				return nil
			end

			function Stat.GetDataFolder(Player: Player)
				if not Data then
					Data = game.ReplicatedStorage.Data
				end

				return Data[Player.Name]
			end

			function Stat.WaitForLoad(Player: any): boolean
				Player = Player or game.Players.LocalPlayer	
				repeat wait() until Player:FindFirstChild("Loaded") and Player.Loaded.Value and Player.Parent ~= nil

				return Player.Parent ~= nil
			end

			return Stat
			
			
			--SERVERSCRIPTSERVICE:
				local ServerScriptService = game:GetService("ServerScriptService")

			local leaderstats = Instance.new("Script")
			leaderstats.Name = "leaderstats"
			leaderstats.Source = "--// Services\nlocal ReplicatedStorage = game:GetService(\'ReplicatedStorage\')\nlocal Players = game:GetService(\'Players\')\n\nlocal Stat = require(ReplicatedStorage.Stat)\n\nPlayers.PlayerAdded:Connect(function(Player)\n	if not Stat.WaitForLoad(Player) then return end -- player left!\n	\n	local MoneyStat = Stat.Get(Player, \'Money\')\n	\n	local Money = Instance.new(\'NumberValue\', Player.leaderstats)\n	Money.Name = \'Money\'\n	Money.Value = MoneyStat.Value\n	\n	MoneyStat.Changed:Connect(function()\n		Money.Value = MoneyStat.Value\n	end)\nend)"
			leaderstats.Parent = ServerScriptService

			local Datastore = Instance.new("Folder")
			Datastore.Name = "Datastore"
			Datastore.Parent = ServerScriptService

			local DataHandler = Instance.new("Script")
			DataHandler.Name = "DataHandler"
			DataHandler.Source = "--// Services\nlocal ReplicatedStorage = game:GetService(\'ReplicatedStorage\')\nlocal Players = game:GetService(\'Players\')\n\n--// Require\nlocal DataManager = require(script.Parent.DataManager)\n\n--// Setup\nlocal DataFolder = Instance.new(\'Folder\', game.ReplicatedStorage)\nDataFolder.Name = \'Data\' -- create data folder\n\n--// Functions\nfunction OnPlayerAdded(Player)\n	local Loaded = Instance.new(\'BoolValue\')\n	Loaded.Name = \'Loaded\'\n	Loaded.Parent = Player\n\n	DataManager.OnPlayerAdded(Player) -- load profile\n	local Folder = DataManager:CreateFolder(Player) -- creates all folders based on profile\n\n	local leaderstats = Instance.new(\'Folder\', Player)\n	leaderstats.Name = \'leaderstats\'\n\n	Loaded.Value = true\n\n	while task.wait(10) do -- upload every 10 seconds (its not like a save, its just so the ProfileService has the data cached)\n		if Player.Parent == nil or Folder.Parent == nil then break end\n		DataManager:FolderToProfile(Player) -- converts a folder to a table and uploads it to the profile\n	end\nend\n\nfunction OnPlayerRemoved(Player)\n	DataManager:FolderToProfile(Player) -- converts a folder to a table and uploads it to profile\n	DataManager.OnPlayerRemoving(Player) -- saves profile\nend\n\n--// Main\nPlayers.PlayerAdded:Connect(OnPlayerAdded)\n\nPlayers.PlayerRemoving:Connect(OnPlayerRemoved)\n\ngame:BindToClose(function()\n	for _, Player in Players:GetPlayers() do\n		OnPlayerRemoved(Player)\n	end\nend)"
			DataHandler.Parent = Datastore

			local DataManager = Instance.new("ModuleScript")
			DataManager.Name = "DataManager"
			DataManager.Source = "--// Services\nlocal ReplicatedStorage = game:GetService(\'ReplicatedStorage\')\nlocal Players = game:GetService(\'Players\')\n\n--// Requires\nlocal ProfileService = require(script.ProfileService)\n\nlocal TempValues = require(script.TempValues)\nlocal Values = require(script.Values)\n\nlocal ProfileTemplate = {}\n\nlocal ProfileStore = ProfileService.GetProfileStore(\n	ReplicatedStorage[\'Game Settings\'].DataSave.Value, \n	ProfileTemplate\n)\n\nlocal Profiles = {}\nlocal DataManager = {}\n\n--// Functions\nlocal function CreateInstance(Type, Name, Parent, Value)\n	local NewInstance = Instance.new(Type)\n	NewInstance.Name = Name\n	NewInstance.Parent = Parent\n\n	if Value then\n		NewInstance.Value = Value\n	end\n\n	return NewInstance\nend\n\n--// Main\nfunction DataManager.OnPlayerAdded(Player)\n	local Profile = ProfileStore:LoadProfileAsync(\n		tostring(Player.UserId),\n		\'ForceLoad\'\n	)\n	\n	--// Load Profile\n	if Profile then\n		Profile:ListenToRelease(function()\n			Profiles[Player] = nil\n			Player:Kick()\n		end)\n		\n		if Player:IsDescendantOf(Players) then			\n			local Data = Profile.Data\n\n			for _,v in Values do\n				if v.Type == \'Folder\' then\n					if v.Parent == \'Player\' then\n						if Data[v.Name] then continue end\n						Data[v.Name] = {}\n					else\n						if Data[v.Parent][v.Name] then continue end\n						Data[v.Parent][v.Name] = {}\n					end\n				else  -- type is a value\n					if v.Parent == \'Player\' then\n						if Data[v.Name] then continue end\n						Data[v.Name] = v.StartingAmount\n					else\n						if Data[v.Parent][v.Name] then continue end\n						Data[v.Parent][v.Name] = v.StartingAmount\n					end\n				end\n			end\n			\n			Profiles[Player] = Profile\n		else\n			Profile:Release()\n		end\n	else\n		Player:Kick()\n	end\n	\n	--// Create TempValues\n	local TempFolder = CreateInstance(\'Folder\', \'TempValues\', Player)\n	\n	for _, TempInfo in TempValues do\n		CreateInstance(TempInfo.Type, TempInfo.Name, TempFolder, TempInfo.StartingAmount)\n	end\nend\n\nfunction DataManager.OnPlayerRemoving(Player)\n	local Profile = Profiles[Player]\n	\n	if Profile then\n		Profile.Data.Other.LastJoin = os.time()\n		Profile:Release()\n	end\nend\n\nfunction DataManager:Get(Player)\n	local Profile = Profiles[Player]\n	\n	if Profile then\n		return Profile.Data\n	end\nend\n\nfunction DataManager:CreateFolder(Player) -- converts a profile to a folder\n	local Data = DataManager:Get(Player)\n	\n	local DataFolder = CreateInstance(\'Folder\', Player.Name, ReplicatedStorage.Data)\n	\n	local function CreateValue(Name, Parent, Value)\n		if type(Value) == \'number\' then\n			return CreateInstance(\'NumberValue\', Name, Parent, Value)\n		elseif type(Value) == \'string\' then\n			return CreateInstance(\'StringValue\', Name, Parent, Value)\n		elseif type(Value) == \'boolean\' then\n			return CreateInstance(\'BoolValue\', Name, Parent, Value)\n		end\n	end\n	\n	for Object, ObjectValue in Data do\n		if type(ObjectValue) == \'table\' then\n			CreateInstance(\'Folder\', Object, DataFolder)\n			\n			for Object2, ObjectValue2 in ObjectValue do -- loop thru this folder for the second layer\n				if type(ObjectValue2) == \'table\' then\n					CreateInstance(\'Folder\', Object2, DataFolder[Object])\n					\n					for Object3, ObjectValue3 in ObjectValue2 do\n						CreateValue(Object3, DataFolder[Object][Object2], ObjectValue3)\n					end					\n				else\n					CreateValue(Object2, DataFolder[Object], ObjectValue2)\n				end\n			end\n		else\n			CreateValue(Object, DataFolder, ObjectValue) -- its a value directly inside data, so save\n		end\n	end\n	\n	return DataFolder\nend\n\nfunction DataManager:FolderToProfile(Player)\n	local DataFolder = ReplicatedStorage.Data[Player.Name]\n	local Data = DataManager:Get(Player)\n	\n	for _, Object in DataFolder:GetChildren() do\n		if Object:IsA(\'Folder\') then\n			Data[Object.Name] = {}\n			\n			for _, ObjectInside in Object:GetChildren() do -- if its a folder, get the things inside\n				if ObjectInside:IsA(\'Folder\') then -- for example the pets\n					Data[Object.Name][ObjectInside.Name] = {}\n					for _, ObjectInside2 in ObjectInside:GetChildren() do -- if its a folder in a folder, do the same but one layer deeper\n						Data[Object.Name][ObjectInside.Name][ObjectInside2.Name] = ObjectInside2.Value\n					end\n				else\n					Data[Object.Name][ObjectInside.Name] = ObjectInside.Value\n				end\n			end\n		else\n			Data[Object.Name] = Object.Value\n		end\n	end	\nend\n\nreturn DataManager"
			DataManager.Parent = Datastore

			local Values = Instance.new("ModuleScript")
			Values.Name = "Values"
			Values.Source = " return { \n	--// Folders\n	{Name = \'Stats\', Parent = \'Player\', Type = \'Folder\'},\n	{Name = \'Buttons\', Parent = \'Player\', Type = \'Folder\'},\n	{Name = \'Other\', Parent = \'Player\', Type = \'Folder\'},\n\n	--// Main Stats \n	{Name = \'Money\', Parent = \'Stats\', Type = \'NumberValue\', StartingAmount = 0},\n	{Name = \'Rebirth\', Parent = \'Stats\', Type = \'NumberValue\', StartingAmount = 0},\n	\n	--// Other\n	{Name = \'LastJoin\', Parent = \'Other\', Type = \'NumberValue\', StartingAmount = 0},\n}"
			Values.Parent = DataManager

			local TempValues = Instance.new("ModuleScript")
			TempValues.Name = "TempValues"
			TempValues.Source = "return { \n	{Name = \'Plot\', Type = \'IntValue\', StartingAmount = 0},\n}"
			TempValues.Parent = DataManager

			local ProfileService = Instance.new("ModuleScript")
			-- The source or text of this instance exceeded the character limit
			ProfileService.Parent = DataManager

			local RemoteHandler = Instance.new("Script")
			RemoteHandler.Name = "RemoteHandler"
			RemoteHandler.Source = "--// Services\nlocal ReplicatedStorage = game:GetService(\'ReplicatedStorage\')\n\n--// Requires\nlocal Stat = require(ReplicatedStorage.Stat)\n\n--// Variables\nlocal Remotes = ReplicatedStorage.RemoteEvents\n\nRemotes.BuyRebirth.OnServerEvent:Connect(function(Player) -- Needs a debounce\n	local Money = Stat.Get(Player, \'Money\')\n	local Rebirth = Stat.Get(Player, \'Rebirth\')\n	\n	local RebirthPrice = ReplicatedStorage[\'Game Settings\'].Balancing.RebirthPrice.Value\n	\n	if Money.Value >= RebirthPrice * (Rebirth.Value + 1) then\n		Money.Value = 0\n		\n		local AmountOfButtons = #ReplicatedStorage.TemplatePlot.Buttons:GetChildren()\n		for i = 1, AmountOfButtons do\n			Stat.Get(Player, \'Button\'..i).Value = false	\n		end\n		\n		Rebirth.Value += 1\n		\n		-- Clear Drops\n		local PlayerDropperPartsFolder = workspace.DropperParts:FindFirstChild(Player.Name .. \'-DropperParts\')\n		\n		for _, Drop in PlayerDropperPartsFolder:GetChildren() do\n			Drop:Destroy()\n		end\n	end\nend)"
			RemoteHandler.Parent = ServerScriptService
			
			local PlotHandler = Instance.new("Script")
			PlotHandler.Name = "PlotHandler"
			PlotHandler.Source = "--// Services\nlocal MarketPlaceService = game:GetService(\'MarketplaceService\')\nlocal ReplicatedStorage = game:GetService(\'ReplicatedStorage\')\nlocal Players = game:GetService(\'Players\')\n\n--// Requires\nlocal Multipliers = require(ReplicatedStorage.Multipliers)\nlocal Stat = require(ReplicatedStorage.Stat)\n\n--// Variables\nlocal Plots = workspace.Plots\nlocal DropperParts\n\nlocal TemplatePlot = ReplicatedStorage.TemplatePlot\n\nlocal GameType = ReplicatedStorage[\'Game Settings\'].GameType.Value\n\n--// Functions\nlocal function MoveButton(Button, Plot)\n	local RelativeCFrame = TemplatePlot.Ground.CFrame:ToObjectSpace(Button.CFrame)\n	Button.CFrame = Plot.Ground.CFrame:ToWorldSpace(RelativeCFrame)\nend\n\nlocal function HideButton(Button) -- Edit this if you have a different button model!\n	Button.Transparency = 1\n	Button.CanCollide = false\n	Button.BillboardGui.Enabled = false\n	Button.CanTouch = false\nend\n\nlocal function ShowButton(Button) -- Edit this if you have a different button model!\n	Button.Transparency = 0\n	Button.CanCollide = true\n	Button.BillboardGui.Enabled = true\n	Button.CanTouch = true\nend\n\nlocal function MoveUpgrade(Upgrade, Plot)\n	local RelativeCFrame = TemplatePlot.Ground.CFrame:ToObjectSpace(Upgrade:GetPivot())\n	Upgrade:PivotTo(Plot.Ground.CFrame:ToWorldSpace(RelativeCFrame))\nend\n\nlocal function LoadPlot(Player, Plot)\n	if not Plots:FindFirstChild(Plot) then return end\n\n	for i = 1, #TemplatePlot.Buttons:GetChildren() do\n		local Button = Stat.Get(Player, \'Button\'..i)\n\n		if not Button.Value then\n			local NewButton = TemplatePlot.Buttons[i]:Clone()\n			MoveButton(NewButton, Plots[Plot])\n			NewButton.BillboardGui.Price.Text = \'$\'..NewButton.Price.Value\n			NewButton.Parent = Plots[Plot].Buttons\n\n			if ReplicatedStorage[\'Game Settings\'].GameType.Value == \'Modern\' then \n				NewButton.BillboardGui.Income.Text = `+{NewButton.Income.Value}$ /s` 	\n			end\n\n			if NewButton.UnlockedByButton.Value ~= 0 then -- Button isn't unlocked from the start	\n				local CanSee = Stat.Get(Player, \'Button\'..NewButton.UnlockedByButton.Value)\n\n				if not CanSee.Value then -- If the player can not see this then hide the button\n					HideButton(NewButton)\n\n					--// This code waits until you unlocked the necessary button and then makes this one visible again\n					local Connection\n					Connection = CanSee.Changed:Connect(function()\n						ShowButton(NewButton)\n						Connection:Disconnect()\n					end)\n				end\n			end\n\n			local Touched = false\n			NewButton.Touched:Connect(function(Hit)\n				if Touched then return end\n				if not Hit.Parent:FindFirstChild(\'Humanoid\') then return end\n				if Players:GetPlayerFromCharacter(Hit.Parent) == Player then\n					local Currency = Stat.Get(Player, \'Money\')\n					if Currency.Value < NewButton.Price.Value then return end -- Can't afford it!\n					Touched = true\n\n					--// Make the data change\n					Currency.Value -= NewButton.Price.Value\n					Button.Value = true\n\n					--// Make the actual tycoon change\n					local NewUpgrade = TemplatePlot.Upgrades[i]:Clone()\n					MoveUpgrade(NewUpgrade, Plots[Plot])\n					NewUpgrade.Parent = Plots[Plot].Upgrades		\n					NewButton:Destroy()\n\n					if NewUpgrade:FindFirstChild(\'Conveyor\') then\n						NewUpgrade.Conveyor.ConveyorScript.Enabled = true\n					elseif NewUpgrade:FindFirstChild(\'Killpart\') then\n						NewUpgrade.KillHandler.Enabled = true\n					end\n				end\n			end)\n		else\n			local NewUpgrade = TemplatePlot.Upgrades[i]:Clone()\n			MoveUpgrade(NewUpgrade, Plots[Plot])\n			NewUpgrade.Parent = Plots[Plot].Upgrades\n\n			if NewUpgrade:FindFirstChild(\'Conveyor\') then\n				NewUpgrade.Conveyor.ConveyorScript.Enabled = true\n			elseif NewUpgrade:FindFirstChild(\'Killpart\') then\n				NewUpgrade.KillHandler.Enabled = true\n			end\n		end\n	end\n\n	for i = 1, #TemplatePlot.RobuxButtons:GetChildren() do\n		local NewButton = TemplatePlot.RobuxButtons[i]:Clone()\n		MoveButton(NewButton, Plots[Plot])\n\n		local Info = MarketPlaceService:GetProductInfo(NewButton.ProductId.Value, Enum.InfoType.Product)\n		NewButton.BillboardGui.Price.Text = Info.PriceInRobux.. \' Robux\'		\n		NewButton.Parent = Plots[Plot].RobuxButtons\n\n		NewButton.Touched:Connect(function(Hit)\n			if Hit.Parent:FindFirstChild(\'Humanoid\') and Players:GetPlayerFromCharacter(Hit.Parent) == Player then\n				MarketPlaceService:PromptProductPurchase(Player, NewButton.ProductId.Value)\n			end\n		end)\n	end\nend\n\nlocal function ClearPlot(Plot)\n	Plot = Plots[Plot]\n\n	for _, Button in Plot.Buttons:GetChildren() do\n		Button:Destroy()\n	end\n\n	for _, RobuxButton in Plot.RobuxButtons:GetChildren() do\n		RobuxButton:Destroy()\n	end\n\n	for _, Upgrade in Plot.Upgrades:GetChildren() do\n		Upgrade:Destroy()\n	end\nend \n\n--// Player stuff ig\nlocal function OnPlayerRemoving(Player)\n	local Plot = Player.TempValues.Plot.Value\n	if Plot == 0 then return end -- Player has no plot\n\n	local PlotInstance = Plots[Plot]\n	PlotInstance.Claimed.Value = \'None\'\n	PlotInstance.Door.Claim.SurfaceGui.TextLabel.Text = \'Claim\'\n\n	ClearPlot(Plot)\n	Player.TempValues.Plot.Value = 0\n\n	-- Remove player's DropperParts folder\n	local PlayerDropperPartsFolder = workspace.DropperParts:FindFirstChild(Player.Name .. \'-DropperParts\')\n	if PlayerDropperPartsFolder then\n		PlayerDropperPartsFolder:Destroy()\n	end\nend\n\nlocal function OnPlayerAdded(Player)\n	if not Stat.WaitForLoad(Player) then return end -- player left!\n\n	local Plot = Player.TempValues.Plot\n\n	Plot.Changed:Connect(function()\n		LoadPlot(Player, Plot.Value)\n	end)\n\n	Stat.Get(Player, \'Rebirth\').Changed:Connect(function()\n		ClearPlot(Plot.Value)\n		LoadPlot(Player, Plot.Value)\n	end)\n\n	-- Create Button Values\n	for i = 1, #TemplatePlot.Buttons:GetChildren() do\n		if not Stat.Get(Player, \'Button\'..i) then\n			local NewButton = Instance.new(\'BoolValue\')\n			NewButton.Name = \'Button\'..i\n			NewButton.Parent = Stat.GetDataFolder(Player).Buttons\n		end\n	end\n\n	if GameType == \'Classic\' then\n		-- Create DropperParts folder for player\n		local PlayerDropperPartsFolder = Instance.new(\'Folder\')\n		PlayerDropperPartsFolder.Name = Player.Name .. \'-DropperParts\'\n		PlayerDropperPartsFolder.Parent = DropperParts\n	elseif GameType == \'Modern\' then\n		-- For modern tycoons, different income system\n\n		local TemplateButtons = ReplicatedStorage.TemplatePlot.Buttons:GetChildren()\n\n		while task.wait(1) do\n			if Player.Parent == nil then break end\n			if Player.TempValues.Plot.Value == 0 then continue end -- Player hasn't claimed a tycoon\n\n			local Income = 0\n\n			for _, Button in TemplateButtons do\n				if not Stat.Get(Player, \'Button\'..Button.Name).Value then continue end -- Player doesn't own this\n\n				Income += Button.Income.Value\n			end\n\n			local Currency = Stat.Get(Player, \'Money\')\n			local Rebirth = Stat.Get(Player, \'Rebirth\')\n			Currency.Value += Income * Multipliers.GetMoneyMultiplier(Player)\n		end\n	end\nend\n\n--// Doors\nlocal function CreateDoor(v, Hit)\n	if v.Claimed.Value ~= \'None\' then return end -- Already Claimed\n\n	if Hit.Parent:FindFirstChild(\'Humanoid\') then -- Check if it is a player\n		local Player = Players:GetPlayerFromCharacter(Hit.Parent)\n\n		if Player.TempValues.Plot.Value ~= 0 then return end -- Player already claimed a plot\n\n		--// Update tycoon so it become's the player's\n		Player.TempValues.Plot.Value = tonumber(v.Name)\n		v.Claimed.Value = Player.Name\n		v.Door.Claim.SurfaceGui.TextLabel.Text = Player.Name..\''s Plot\'\n	end\nend\n\nlocal function CreateDoors()\n	for _,v in Plots:GetChildren() do\n		v.Door.Claim.Touched:Connect(function(Hit)\n			CreateDoor(v, Hit)\n		end)\n	end\nend\n\n--// Dropper Parts Folder\nlocal function CreateDropperPartsFolder()\n	if GameType == \'Classic\' then\n		DropperParts = Instance.new(\'Folder\')\n		DropperParts.Name = \'DropperParts\'\n		DropperParts.Parent = workspace\n	end\nend\n\n--// Calls\nCreateDoors()\nCreateDropperPartsFolder()\n\n--// Connections\nPlayers.PlayerAdded:Connect(OnPlayerAdded)\nPlayers.PlayerRemoving:Connect(OnPlayerRemoving)"
			PlotHandler.Parent = ServerScriptService

			local Dropper = Instance.new("ModuleScript")
			Dropper.Name = "Dropper"
			Dropper.Source = "local Dropper = {}\n\nlocal Stat = require(game.ReplicatedStorage.Stat)\nlocal Multipliers = require(game.ReplicatedStorage.Multipliers)\n\nfunction Dropper.Spawn(Player, Pos, Amount)\n	local NewPart = Instance.new(\'Part\')\n	NewPart.Size = Vector3.new(1,1,1)\n	NewPart.Position = Pos\n	NewPart.Parent = workspace.DropperParts[Player.Name..\'-DropperParts\']\n	\n	local Worth = Instance.new(\'NumberValue\')\n	Worth.Name = \'Worth\'\n	Worth.Value = Amount\n	Worth.Parent = NewPart\n	\n	local Billboard = script.BillboardGui:Clone()\n	Billboard.TextLabel.Text = \'$\'..Worth.Value\n	Billboard.Parent = NewPart\n	\n	Worth.Changed:Connect(function()\n		Billboard.TextLabel.Text = \'$\'..Worth.Value\n	end)\n	\n	task.spawn(function() -- Despawn after 30 seconds\n		task.wait(30)\n		NewPart:Destroy()\n	end)\n	\n	local Currency = Stat.Get(Player, \'Money\')\n	local Rebirth = Stat.Get(Player, \'Rebirth\')\n	\n	NewPart.Touched:Connect(function(Hit)\n		if Hit.Name == \'Furnace\' then\n			Currency.Value += Worth.Value * Multipliers.GetMoneyMultiplier(Player)\n			NewPart:Destroy()\n		elseif Hit.Name == \'Ground\' then\n			NewPart:Destroy()\n		end\n	end)\nend\n\nreturn Dropper"
			Dropper.Parent = ServerScriptService

			local BillboardGui = Instance.new("BillboardGui")
			BillboardGui.Active = true
			BillboardGui.LightInfluence = 1
			BillboardGui.Size = UDim2.new(1.80, 0.00, 0.90, 0.00)
			BillboardGui.ClipsDescendants = true
			BillboardGui.MaxDistance = 25
			BillboardGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
			BillboardGui.StudsOffset = Vector3.new(0.00, 1.20, 0.00)
			BillboardGui.Parent = Dropper

			local TextLabel = Instance.new("TextLabel")
			TextLabel.TextWrapped = true
			TextLabel.BorderSizePixel = 0
			TextLabel.TextScaled = true
			TextLabel.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			TextLabel.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			TextLabel.TextSize = 14
			TextLabel.Size = UDim2.new(1.00, 0.00, 1.00, 0.00)
			TextLabel.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			TextLabel.Text = "$100"
			TextLabel.TextColor3 = Color3.new(0.33, 1.00, 0.00)
			TextLabel.BackgroundTransparency = 1
			TextLabel.Parent = BillboardGui

			local UIStroke = Instance.new("UIStroke")
			UIStroke.Color = Color3.new(0.11, 0.33, 0.00)
			UIStroke.Thickness = 2
			UIStroke.Parent = TextLabel

			local RobuxHandler = Instance.new("Script")
			RobuxHandler.Name = "RobuxHandler"
			RobuxHandler.Source = "--// Services\nlocal MarketPlaceService = game:GetService(\'MarketplaceService\')\nlocal ReplicatedStorage = game:GetService(\'ReplicatedStorage\')\nlocal Players = game:GetService(\'Players\')\n\n--// Imports\nlocal Stat = require(ReplicatedStorage.Stat)\n\n--// Variables\nlocal GamepassIds = ReplicatedStorage.GamepassIds\n\n--// Functions\nlocal function AwardTool(Player, ToolName)\n	local Tool = script:FindFirstChild(ToolName):Clone()\n\n	if not Tool then\n		warn(\'Error awarding gamepass reward, \'..ToolName..\' does not exist!\')\n		return -- An error occured, stop the function from running\n	end\n\n	Tool:Clone().Parent = Player.Backpack	\nend\n\nlocal function CreateGamepasses(Player)\n	local Data = Stat.GetDataFolder(Player)\n	for _, GamepassInstance in GamepassIds:GetChildren() do\n		local GPVal = Data.Other:FindFirstChild(GamepassInstance.Name)\n\n		-- Create a gamepass if it doesn't exist\n		if not GPVal then\n			GPVal = Instance.new(\'BoolValue\')\n			GPVal.Name = GamepassInstance.Name\n			GPVal.Parent = Data.Other\n		end\n\n		if MarketPlaceService:UserOwnsGamePassAsync(Player.UserId, GamepassInstance.Value) then\n			GPVal.Value = true\n		end \n	end\nend\n\nlocal function OnCharacterAdded(Character) -- Function loads in the tools\n	local Player = Players:GetPlayerFromCharacter(Character)\n\n	for _, GamepassInstance in GamepassIds:GetChildren() do\n		if not script:FindFirstChild(GamepassInstance.Name) then continue end -- Gamepass has no tool\n\n		if Stat.Get(Player, GamepassInstance.Name).Value == false then continue end\n\n		AwardTool(Player, GamepassInstance.Name)\n	end\nend\n\nfunction OnPlayerAdded(Player)\n	Stat.WaitForLoad(Player)\n	CreateGamepasses(Player) -- Creates the values\n\n	local Character = Player.Character or Player.CharacterAdded:Wait()\n\n	Player.CharacterAdded:Connect(OnCharacterAdded)\n	OnCharacterAdded(Character)\nend\n\nfunction OnGamepassPurchaseFinished(Player, GamepassId, Purchased)\n	if not Purchased then return end\n\n	for _, GamepassInstance in GamepassIds:GetChildren() do\n		if GamepassInstance.Value == GamepassId then\n			AwardTool(Player, GamepassInstance.Name)\n			break\n		end\n	end\nend\n\nfunction ProcessReceipt(ReceiptInfo)\n	local Player = Players:GetPlayerByUserId(ReceiptInfo.PlayerId)\n\n	for _, Button in ReplicatedStorage.TemplatePlot.RobuxButtons:GetChildren() do\n		if Button.ProductId.Value == ReceiptInfo.ProductId then\n			local Amount = Button.Amount.Value\n			local Money = Stat.Get(Player, \'Money\')\n			Money.Value += Amount\n			break\n		end\n	end\n\n	return Enum.ProductPurchaseDecision.PurchaseGranted\nend\n\n--// Main\nPlayers.PlayerAdded:Connect(OnPlayerAdded)\n\nMarketPlaceService.PromptGamePassPurchaseFinished:Connect(OnGamepassPurchaseFinished)\n\nMarketPlaceService.ProcessReceipt = ProcessReceipt"
			RobuxHandler.Parent = ServerScriptService

			local LaserGun = Instance.new("Tool")
			LaserGun.Name = "LaserGun"
			LaserGun.GripPos = Vector3.new(0.00, -0.10, 0.75)
			LaserGun.TextureId = "http://www.roblox.com/asset/?id=130093050"
			LaserGun.CanBeDropped = false
			LaserGun.WorldPivot = CFrame.new(-51.27, 1.70, 83.07, 0.17, 0.44, 0.88)
			LaserGun.Grip = CFrame.new(0.00, -0.10, 0.75, -0.00, -0.00, -1.00)
			LaserGun.Parent = RobuxHandler

			local Handle = Instance.new("Part")
			Handle.Name = "Handle"
			Handle.TopSurface = Enum.SurfaceType.Smooth
			Handle.Size = Vector3.new(0.58, 1.34, 2.48)
			Handle.BottomSurface = Enum.SurfaceType.Smooth
			Handle.Rotation = Vector3.new(153.54, -9.77, -163.44)
			Handle.BrickColor = BrickColor.new("Medium stone grey")
			Handle.Position = Vector3.new(-51.27, 1.70, 83.07)
			Handle.CFrame = CFrame.new(-51.27, 1.70, 83.07, 0.17, 0.44, 0.88)
			Handle.Parent = LaserGun

			local Mesh = Instance.new("SpecialMesh")
			Mesh.Name = "Mesh"
			Mesh.MeshType = Enum.MeshType.FileMesh
			Mesh.Scale = Vector3.new(0.65, 0.65, 0.65)
			Mesh.MeshId = "http://www.roblox.com/asset/?id=130099641"
			Mesh.TextureId = "http://www.roblox.com/asset/?id=130093033"
			Mesh.Parent = Handle

			local Fire = Instance.new("Sound")
			Fire.Name = "Fire"
			Fire.SoundId = "http://www.roblox.com/asset?id=130113322"
			Fire.Parent = Handle
			
			local Reload = Instance.new("Sound")
			Reload.Name = "Reload"
			Reload.SoundId = "http://www.roblox.com/asset?id=130113370"
			Reload.Parent = Handle

			local PointLight = Instance.new("PointLight")
			PointLight.Color = Color3.new(0.00, 1.00, 1.00)
			PointLight.Range = 6
			PointLight.Parent = Handle

			local HitFade = Instance.new("Sound")
			HitFade.Name = "HitFade"
			HitFade.SoundId = "http://www.roblox.com/asset?id=130113415"
			HitFade.Parent = Handle

			local ToolScript = Instance.new("LocalScript")
			ToolScript.Name = "ToolScript"
			ToolScript.Source = "--Rescripted by Luckymaxer\n\nTool = script.Parent\nHandle = Tool:WaitForChild(\'Handle\')\n\nPlayers = game:GetService(\'Players\')\n\nServerControl = Tool:WaitForChild(\'ServerControl\')\nClientControl = Tool:WaitForChild(\'ClientControl\')\n\nClientControl.OnClientInvoke = (function(Mode, Value)\n	if Mode == \'PlaySound\' and Value then\n		Value:Play()\n	end\nend)\n\nfunction InvokeServer(Mode, Value, arg)\n	pcall(function()\n		ServerControl:InvokeServer(Mode, Value, arg)\n	end)\nend\n\nfunction Equipped(Mouse)\n	Character = Tool.Parent\n	Player = Players:GetPlayerFromCharacter(Character)\n	Humanoid = Character:FindFirstChild(\'Humanoid\')\n	if not Player or not Humanoid or Humanoid.Health == 0 then\n		return\n	end\n	Mouse.Button1Down:connect(function()\n		InvokeServer(\'Click\', true, Mouse.Hit.p)\n	end)\nend\n\nlocal function Unequipped()\n	\nend\n\nTool.Equipped:connect(Equipped)\nTool.Unequipped:connect(Unequipped)"
			ToolScript.Parent = LaserGun

			local MouseIcon = Instance.new("LocalScript")
			MouseIcon.Name = "MouseIcon"
			MouseIcon.Source = "local MOUSE_ICON = 'rbxasset://textures/GunCursor.png'\nlocal RELOADING_ICON = 'rbxasset://textures/GunWaitCursor.png'\n\nlocal Tool = script.Parent\n\nlocal Mouse = nil\n\nlocal function UpdateIcon()\n	if Mouse then\n		Mouse.Icon = Tool.Enabled and MOUSE_ICON or RELOADING_ICON\n	end\nend\n\nlocal function OnEquipped(mouse)\n	Mouse = mouse\n	UpdateIcon()\nend\n\nlocal function OnChanged(property)\n	if property == 'Enabled' then\n		UpdateIcon()\n	end\nend\n\nTool.Equipped:connect(OnEquipped)\nTool.Changed:connect(OnChanged)\n"
			MouseIcon.Parent = LaserGun

			local Script = Instance.new("Script")
			Script.Source = "--Rescripted by Luckymaxer\n\nTool = script.Parent\nHandle = Tool:WaitForChild(\'Handle\')\n\nPlayers = game:GetService(\'Players\')\nDebris = game:GetService(\'Debris\')\n\nSpeed = 100\nDuration = 1\n\nNozzleOffset = Vector3.new(0, 0.4, -1.1)\n\nSounds = {\n	Fire = Handle:WaitForChild(\'Fire\'),\n	Reload = Handle:WaitForChild(\'Reload\'),\n	HitFade = Handle:WaitForChild(\'HitFade\')\n}\n\nPointLight = Handle:WaitForChild(\'PointLight\')\n\nServerControl = (Tool:FindFirstChild(\'ServerControl\') or Instance.new(\'RemoteFunction\'))\nServerControl.Name = \'ServerControl\'\nServerControl.Parent = Tool\n\nClientControl = (Tool:FindFirstChild(\'ClientControl\') or Instance.new(\'RemoteFunction\'))\nClientControl.Name = \'ClientControl\'\nClientControl.Parent = Tool\n\nServerControl.OnServerInvoke = (function(player, Mode, Value, arg)\n	if player ~= Player or Humanoid.Health == 0 or not Tool.Enabled then\n		return\n	end\n	if Mode == \'Click\' and Value then\n		Activated(arg)\n	end\nend)\n\nfunction InvokeClient(Mode, Value)\n	pcall(function()\n		ClientControl:InvokeClient(Player, Mode, Value)\n	end)\nend\n\nfunction TagHumanoid(humanoid, player)\n	local Creator_Tag = Instance.new(\'ObjectValue\')\n	Creator_Tag.Name = \'creator\'\n	Creator_Tag.Value = player\n	Debris:AddItem(Creator_Tag, 2)\n	Creator_Tag.Parent = humanoid\nend\n\nfunction UntagHumanoid(humanoid)\n	for i, v in pairs(humanoid:GetChildren()) do\n		if v:IsA(\'ObjectValue\') and v.Name == \'creator\' then\n			v:Destroy()\n		end\n	end\nend\n\nfunction FindCharacterAncestor(Parent)\n	if Parent and Parent ~= game:GetService(\'Workspace\') then\n		local humanoid = Parent:FindFirstChild(\'Humanoid\')\n		if humanoid then\n			return Parent, humanoid\n		else\n			return FindCharacterAncestor(Parent.Parent)\n		end\n	end\n	return nil\nend\n\nfunction GetTransparentsRecursive(Parent, PartsTable)\n	local PartsTable = (PartsTable or {})\n	for i, v in pairs(Parent:GetChildren()) do\n		local TransparencyExists = false\n		pcall(function()\n			local Transparency = v[\'Transparency\']\n			if Transparency then\n				TransparencyExists = true\n			end\n		end)\n		if TransparencyExists then\n			table.insert(PartsTable, v)\n		end\n		GetTransparentsRecursive(v, PartsTable)\n	end\n	return PartsTable\nend\n\nfunction SelectionBoxify(Object)\n	local SelectionBox = Instance.new(\'SelectionBox\')\n	SelectionBox.Adornee = Object\n	SelectionBox.Color = BrickColor.new(\'Toothpaste\')\n	SelectionBox.Parent = Object\n	return SelectionBox\nend\n\nlocal function Light(Object)\n	local Light = PointLight:Clone()\n	Light.Range = (Light.Range + 2)\n	Light.Parent = Object\nend\n\nfunction FadeOutObjects(Objects, FadeIncrement)\n	repeat\n		local LastObject = nil\n		for i, v in pairs(Objects) do\n			v.Transparency = (v.Transparency + FadeIncrement)\n			LastObject = v\n		end\n		wait()\n	until LastObject.Transparency >= 1 or not LastObject\nend\n\nfunction Dematerialize(character, humanoid, FirstPart)\n	if not character or not humanoid then\n		return\n	end\n	\n	humanoid.WalkSpeed = 0\n\n	local Parts = {}\n	\n	for i, v in pairs(character:GetChildren()) do\n		if v:IsA(\'BasePart\') then\n			v.Anchored = true\n			table.insert(Parts, v)\n		elseif v:IsA(\'LocalScript\') or v:IsA(\'Script\') then\n			v:Destroy()\n		end\n	end\n\n	local SelectionBoxes = {}\n\n	local FirstSelectionBox = SelectionBoxify(FirstPart)\n	Light(FirstPart)\n	wait(0.05)\n\n	for i, v in pairs(Parts) do\n		if v ~= FirstPart then\n			table.insert(SelectionBoxes, SelectionBoxify(v))\n			Light(v)\n		end\n	end\n\n	local ObjectsWithTransparency = GetTransparentsRecursive(character)\n	FadeOutObjects(ObjectsWithTransparency, 0.1)\n\n	wait(0.5)\n\n	character:BreakJoints()\n	humanoid.Health = 0\n	\n	Debris:AddItem(character, 2)\n\n	local FadeIncrement = 0.05\n	Delay(0.2, function()\n		FadeOutObjects({FirstSelectionBox}, FadeIncrement)\n		if character and character.Parent then\n			character:Destroy()\n		end\n	end)\n	FadeOutObjects(SelectionBoxes, FadeIncrement)\nend\n\nfunction Touched(Projectile, Hit)\n	if not Hit or not Hit.Parent then\n		return\n	end\n	local character, humanoid = FindCharacterAncestor(Hit)\n	if character and humanoid and character ~= Character then\n		local ForceFieldExists = false\n		for i, v in pairs(character:GetChildren()) do\n			if v:IsA(\'ForceField\') then\n				ForceFieldExists = true\n			end\n		end\n		if not ForceFieldExists then\n			if Projectile then\n				local HitFadeSound = Projectile:FindFirstChild(Sounds.HitFade.Name)\n				local torso = humanoid.Torso\n				if HitFadeSound and torso then\n					HitFadeSound.Parent = torso\n					HitFadeSound:Play()\n				end\n			end\n			Dematerialize(character, humanoid, Hit)\n		end\n		if Projectile and Projectile.Parent then\n			Projectile:Destroy()\n		end\n	end\nend\n\nfunction Equipped()\n	Character = Tool.Parent\n	Player = Players:GetPlayerFromCharacter(Character)\n	Humanoid = Character:FindFirstChild(\'Humanoid\')\n	if not Player or not Humanoid or Humanoid.Health == 0 then\n		return\n	end\nend\n\nfunction Activated(target)\n	if Tool.Enabled and Humanoid.Health > 0 then\n		Tool.Enabled = false\n\n		InvokeClient(\'PlaySound\', Sounds.Fire)\n\n		local HandleCFrame = Handle.CFrame\n		local FiringPoint = HandleCFrame.p + HandleCFrame:vectorToWorldSpace(NozzleOffset)\n		local ShotCFrame = CFrame.new(FiringPoint, target)\n\n		local LaserShotClone = BaseShot:Clone()\n		LaserShotClone.CFrame = ShotCFrame + (ShotCFrame.lookVector * (BaseShot.Size.Z / 2))\n		local BodyVelocity = Instance.new(\'BodyVelocity\')\n		BodyVelocity.velocity = ShotCFrame.lookVector * Speed\n		BodyVelocity.Parent = LaserShotClone\n		LaserShotClone.Touched:connect(function(Hit)\n			if not Hit or not Hit.Parent then\n				return\n			end\n			Touched(LaserShotClone, Hit)\n		end)\n		Debris:AddItem(LaserShotClone, Duration)\n		LaserShotClone.Parent = game:GetService(\'Workspace\')\n\n		wait(0.6) -- FireSound length\n\n		InvokeClient(\'PlaySound\', Sounds.Reload)\n		\n		wait(0.75) -- ReloadSound length\n\n		Tool.Enabled = true\n	end\nend\n\nfunction Unequipped()\n	\nend\n\nBaseShot = Instance.new(\'Part\')\nBaseShot.Name = \'Effect\'\nBaseShot.BrickColor = BrickColor.new(\'Toothpaste\')\nBaseShot.Material = Enum.Material.Plastic\nBaseShot.Shape = Enum.PartType.Block\nBaseShot.TopSurface = Enum.SurfaceType.Smooth\nBaseShot.BottomSurface = Enum.SurfaceType.Smooth\nBaseShot.FormFactor = Enum.FormFactor.Custom\nBaseShot.Size = Vector3.new(0.2, 0.2, 3)\nBaseShot.CanCollide = false\nBaseShot.Locked = true\nSelectionBoxify(BaseShot)\nLight(BaseShot)\nBaseShotSound = Sounds.HitFade:Clone()\nBaseShotSound.Parent = BaseShot\n\nTool.Equipped:connect(Equipped)\nTool.Unequipped:connect(Unequipped)"
			Script.Parent = LaserGun

			local ServerControl = Instance.new("RemoteFunction")
			ServerControl.Name = "ServerControl"
			ServerControl.Parent = LaserGun

			local ClientControl = Instance.new("RemoteFunction")
			ClientControl.Name = "ClientControl"
			ClientControl.Parent = LaserGun

			local Sword = Instance.new("Tool")
			Sword.Name = "Sword"
			Sword.GripPos = Vector3.new(0.00, 0.00, -1.70)
			Sword.GripUp = Vector3.new(0.00, 0.00, 1.00)
			Sword.GripRight = Vector3.new(0.00, 1.00, 0.00)
			Sword.TextureId = "rbxasset://Textures/Sword128.png"
			Sword.GripForward = Vector3.new(-1.00, -0.00, -0.00)
			Sword.WorldPivot = CFrame.new(-98.60, 2.39, 89.32, -0.46, -0.72, -0.51)
			Sword.Grip = CFrame.new(0.00, 0.00, -1.70, -1.00, -0.00, -0.00)
			Sword.Parent = RobuxHandler

			local Handle_1 = Instance.new("Part")
			Handle_1.Name = "Handle"
			Handle_1.TopSurface = Enum.SurfaceType.Smooth
			Handle_1.Color = Color3.new(0.39, 0.37, 0.38)
			Handle_1.Locked = true
			Handle_1.Size = Vector3.new(1.00, 0.80, 4.00)
			Handle_1.BottomSurface = Enum.SurfaceType.Smooth
			Handle_1.Rotation = Vector3.new(-54.62, 27.65, 84.10)
			Handle_1.BrickColor = BrickColor.new("Dark stone grey")
			Handle_1.Position = Vector3.new(-98.60, 2.39, 89.32)
			Handle_1.Reflectance = 0.4000000059604645
			Handle_1.CFrame = CFrame.new(-98.60, 2.39, 89.32, -0.46, -0.72, -0.51)
			Handle_1.Parent = Sword

			local Mesh_1 = Instance.new("SpecialMesh")
			Mesh_1.Name = "Mesh"
			Mesh_1.MeshType = Enum.MeshType.FileMesh
			Mesh_1.MeshId = "rbxasset://fonts/sword.mesh"
			Mesh_1.TextureId = "rbxasset://textures/SwordTexture.png"
			Mesh_1.Parent = Handle_1

			local SwordSlash = Instance.new("Sound")
			SwordSlash.Name = "SwordSlash"
			SwordSlash.Volume = 0.699999988079071
			SwordSlash.SoundId = "http://www.roblox.com/asset/?id=12222216"
			SwordSlash.Parent = Handle_1

			local SwordLunge = Instance.new("Sound")
			SwordLunge.Name = "SwordLunge"
			SwordLunge.Volume = 0.6000000238418579
			SwordLunge.SoundId = "http://www.roblox.com/asset/?id=12222208"
			SwordLunge.Parent = Handle_1

			local Unsheath = Instance.new("Sound")
			Unsheath.Name = "Unsheath"
			Unsheath.Volume = 1
			Unsheath.SoundId = "http://www.roblox.com/asset/?id=12222225"
			Unsheath.Parent = Handle_1

			local MouseIcon_1 = Instance.new("LocalScript")
			MouseIcon_1.Name = "MouseIcon"
			MouseIcon_1.Source = "--Made by Luckymaxer\n\nMouse_Icon = \'rbxasset://textures/GunCursor.png\'\nReloading_Icon = \'rbxasset://textures/GunWaitCursor.png\'\n\nTool = script.Parent\n\nMouse = nil\n\nfunction UpdateIcon()\n	if Mouse then\n		Mouse.Icon = Tool.Enabled and Mouse_Icon or Reloading_Icon\n	end\nend\n\nfunction OnEquipped(ToolMouse)\n	Mouse = ToolMouse\n	UpdateIcon()\nend\n\nfunction OnChanged(Property)\n	if Property == \'Enabled\' then\n		UpdateIcon()\n	end\nend\n\nTool.Equipped:Connect(OnEquipped)\nTool.Changed:Connect(OnChanged)\n"
			MouseIcon_1.Parent = Sword
			
			local SwordScript = Instance.new("Script")
			SwordScript.Name = "SwordScript"
			SwordScript.Source = "--Rescripted by Luckymaxer\n--EUROCOW WAS HERE BECAUSE I MADE THE PARTICLES AND THEREFORE THIS ENTIRE SWORD PRETTY AND LOOK PRETTY WORDS AND I'D LIKE TO DEDICATE THIS TO MY FRIENDS AND HI LUCKYMAXER PLS FIX SFOTH SWORDS TY LOVE Y'ALl\n--Updated for R15 avatars by StarWars\n--Re-updated by TakeoHonorable\n\nTool = script.Parent\nHandle = Tool:WaitForChild(\'Handle\')\n\nfunction Create(ty)\n	return function(data)\n		local obj = Instance.new(ty)\n		for k, v in pairs(data) do\n			if type(k) == 'number' then\n				v.Parent = obj\n			else\n				obj[k] = v\n			end\n		end\n		return obj\n	end\nend\n\nlocal BaseUrl = \'rbxassetid://\'\n\nPlayers = game:GetService(\'Players\')\nDebris = game:GetService(\'Debris\')\nRunService = game:GetService(\'RunService\')\n\nDamageValues = {\n	BaseDamage = 5,\n	SlashDamage = 10,\n	LungeDamage = 30\n}\n\n--For R15 avatars\nAnimations = {\n	R15Slash = 522635514,\n	R15Lunge = 522638767\n}\n\nDamage = DamageValues.BaseDamage\n\nGrips = {\n	Up = CFrame.new(0, 0, -1.70000005, 0, 0, 1, 1, 0, 0, 0, 1, 0),\n	Out = CFrame.new(0, 0, -1.70000005, 0, 1, 0, 1, -0, 0, 0, 0, -1)\n}\n\nSounds = {\n	Slash = Handle:WaitForChild(\'SwordSlash\'),\n	Lunge = Handle:WaitForChild(\'SwordLunge\'),\n	Unsheath = Handle:WaitForChild(\'Unsheath\')\n}\n\nToolEquipped = false\n\n--For Omega Rainbow Katana thumbnail to display a lot of particles.\nfor i, v in pairs(Handle:GetChildren()) do\n	if v:IsA(\'ParticleEmitter\') then\n		v.Rate = 20\n	end\nend\n\nTool.Grip = Grips.Up\nTool.Enabled = true\n\nfunction IsTeamMate(Player1, Player2)\n	return (Player1 and Player2 and not Player1.Neutral and not Player2.Neutral and Player1.TeamColor == Player2.TeamColor)\nend\n\nfunction TagHumanoid(humanoid, player)\n	local Creator_Tag = Instance.new(\'ObjectValue\')\n	Creator_Tag.Name = \'creator\'\n	Creator_Tag.Value = player\n	Debris:AddItem(Creator_Tag, 2)\n	Creator_Tag.Parent = humanoid\nend\n\nfunction UntagHumanoid(humanoid)\n	for i, v in pairs(humanoid:GetChildren()) do\n		if v:IsA(\'ObjectValue\') and v.Name == \'creator\' then\n			v:Destroy()\n		end\n	end\nend\n\nfunction Blow(Hit)\n	if not Hit or not Hit.Parent or not CheckIfAlive() or not ToolEquipped then\n		return\n	end\n	local RightArm = Character:FindFirstChild(\'Right Arm\') or Character:FindFirstChild(\'RightHand\')\n	if not RightArm then\n		return\n	end\n	local RightGrip = RightArm:FindFirstChild(\'RightGrip\')\n	if not RightGrip or (RightGrip.Part0 ~= Handle and RightGrip.Part1 ~= Handle) then\n		return\n	end\n	local character = Hit.Parent\n	if character == Character then\n		return\n	end\n	local humanoid = character:FindFirstChildOfClass(\'Humanoid\')\n	if not humanoid or humanoid.Health == 0 then\n		return\n	end\n	local player = Players:GetPlayerFromCharacter(character)\n	if player and (player == Player or IsTeamMate(Player, player)) then\n		return\n	end\n	UntagHumanoid(humanoid)\n	TagHumanoid(humanoid, Player)\n	humanoid:TakeDamage(Damage)	\nend\n\n\nfunction Attack()\n	Damage = DamageValues.SlashDamage\n	Sounds.Slash:Play()\n\n	if Humanoid then\n		if Humanoid.RigType == Enum.HumanoidRigType.R6 then\n			local Anim = Instance.new(\'StringValue\')\n			Anim.Name = \'toolanim\'\n			Anim.Value = \'Slash\'\n			Anim.Parent = Tool\n		elseif Humanoid.RigType == Enum.HumanoidRigType.R15 then\n			local Anim = Tool:FindFirstChild(\'R15Slash\')\n			if Anim then\n				local Track = Humanoid:LoadAnimation(Anim)\n				Track:Play(0)\n			end\n		end\n	end	\nend\n\nfunction Lunge()\n	Damage = DamageValues.LungeDamage\n\n	Sounds.Lunge:Play()\n	\n	if Humanoid then\n		if Humanoid.RigType == Enum.HumanoidRigType.R6 then\n			local Anim = Instance.new(\'StringValue\')\n			Anim.Name = \'toolanim\'\n			Anim.Value = \'Lunge\'\n			Anim.Parent = Tool\n		elseif Humanoid.RigType == Enum.HumanoidRigType.R15 then\n			local Anim = Tool:FindFirstChild(\'R15Lunge\')\n			if Anim then\n				local Track = Humanoid:LoadAnimation(Anim)\n				Track:Play(0)\n			end\n		end\n	end	\n	--[[\n	if CheckIfAlive() then\n		local Force = Instance.new(\'BodyVelocity\')\n		Force.velocity = Vector3.new(0, 10, 0) \n		Force.maxForce = Vector3.new(0, 4000, 0)\n		Debris:AddItem(Force, 0.4)\n		Force.Parent = Torso\n	end\n	]]\n	\n	wait(0.2)\n	Tool.Grip = Grips.Out\n	wait(0.6)\n	Tool.Grip = Grips.Up\n\n	Damage = DamageValues.SlashDamage\nend\n\nTool.Enabled = true\nLastAttack = 0\n\nfunction Activated()\n	if not Tool.Enabled or not ToolEquipped or not CheckIfAlive() then\n		return\n	end\n	Tool.Enabled = false\n	local Tick = RunService.Stepped:wait()\n	if (Tick - LastAttack < 0.2) then\n		Lunge()\n	else\n		Attack()\n	end\n	LastAttack = Tick\n	--wait(0.5)\n	Damage = DamageValues.BaseDamage\n	local SlashAnim = (Tool:FindFirstChild(\'R15Slash\') or Create(\'Animation\'){\n		Name = \'R15Slash\',\n		AnimationId = BaseUrl .. Animations.R15Slash,\n		Parent = Tool\n	})\n	\n	local LungeAnim = (Tool:FindFirstChild(\'R15Lunge\') or Create(\'Animation\'){\n		Name = \'R15Lunge\',\n		AnimationId = BaseUrl .. Animations.R15Lunge,\n		Parent = Tool\n	})\n	Tool.Enabled = true\nend\n\nfunction CheckIfAlive()\n	return (((Player and Player.Parent and Character and Character.Parent and Humanoid and Humanoid.Parent and Humanoid.Health > 0 and Torso and Torso.Parent) and true) or false)\nend\n\nfunction Equipped()\n	Character = Tool.Parent\n	Player = Players:GetPlayerFromCharacter(Character)\n	Humanoid = Character:FindFirstChildOfClass(\'Humanoid\')\n	Torso = Character:FindFirstChild(\'Torso\') or Character:FindFirstChild(\'HumanoidRootPart\')\n	if not CheckIfAlive() then\n		return\n	end\n	ToolEquipped = true\n	Sounds.Unsheath:Play()\nend\n\nfunction Unequipped()\n	Tool.Grip = Grips.Up\n	ToolEquipped = false\nend\n\nTool.Activated:Connect(Activated)\nTool.Equipped:Connect(Equipped)\nTool.Unequipped:Connect(Unequipped)\n\nConnection = Handle.Touched:Connect(Blow)"
			SwordScript.Parent = Sword

			local SpeedCoil = Instance.new("Tool")
			SpeedCoil.Name = "SpeedCoil"
			SpeedCoil.GripPos = Vector3.new(-0.00, 0.00, -1.00)
			SpeedCoil.GripUp = Vector3.new(-0.71, -0.71, 0.00)
			SpeedCoil.GripRight = Vector3.new(-0.71, 0.71, 0.00)
			SpeedCoil.TextureId = "http://www.roblox.com/asset/?id=99170415"
			SpeedCoil.WorldPivot = CFrame.new(-216.92, 3.79, 104.95, -1.00, 0.03, -0.04)
			SpeedCoil.ToolTip = "Speed Up!"
			SpeedCoil.Grip = CFrame.new(-0.00, 0.00, -1.00, -0.00, -0.00, -1.00)
			SpeedCoil.Parent = RobuxHandler

			local Handle_1 = Instance.new("Part")
			Handle_1.Name = "Handle"
			Handle_1.TopSurface = Enum.SurfaceType.Smooth
			Handle_1.Color = Color3.new(0.77, 0.16, 0.11)
			Handle_1.Locked = true
			Handle_1.Size = Vector3.new(1.30, 1.30, 2.40)
			Handle_1.BottomSurface = Enum.SurfaceType.Smooth
			Handle_1.Rotation = Vector3.new(36.15, 87.50, -172.00)
			Handle_1.BrickColor = BrickColor.new("Bright red")
			Handle_1.Position = Vector3.new(-216.92, 3.79, 104.95)
			Handle_1.CFrame = CFrame.new(-216.92, 3.79, 104.95, -1.00, 0.03, -0.04)
			Handle_1.Parent = SpeedCoil

			local CoilSound = Instance.new("Sound")
			CoilSound.Name = "CoilSound"
			CoilSound.Volume = 1
			CoilSound.SoundId = "http://www.roblox.com/asset/?id=99173388"
			CoilSound.Parent = Handle_1

			local Mesh_1 = Instance.new("SpecialMesh")
			Mesh_1.Name = "Mesh"
			Mesh_1.MeshType = Enum.MeshType.FileMesh
			Mesh_1.Scale = Vector3.new(0.70, 0.70, 0.70)
			Mesh_1.MeshId = "http://www.roblox.com/asset/?id=16606212"
			Mesh_1.TextureId = "http://www.roblox.com/asset/?id=99170547"
			Mesh_1.Parent = Handle_1

			local RightGripAttachment = Instance.new("Attachment")
			RightGripAttachment.Name = "RightGripAttachment"
			RightGripAttachment.WorldOrientation = Vector3.new(1.47, 87.98, -0.87)
			RightGripAttachment.CFrame = CFrame.new(0.00, 0.00, -1.00, -0.00, -0.00, -1.00)
			RightGripAttachment.Axis = Vector3.new(-0.71, 0.71, 0.00)
			RightGripAttachment.WorldAxis = Vector3.new(0.03, -0.02, -1.00)
			RightGripAttachment.SecondaryAxis = Vector3.new(-0.71, -0.71, 0.00)
			RightGripAttachment.Position = Vector3.new(0.00, 0.00, -1.00)
			RightGripAttachment.Orientation = Vector3.new(-0.00, 0.00, 135.00)
			RightGripAttachment.WorldCFrame = CFrame.new(-217.92, 3.81, 104.92, -1.00, 0.03, -0.04)
			RightGripAttachment.WorldPosition = Vector3.new(-217.92, 3.81, 104.92)
			RightGripAttachment.WorldSecondaryAxis = Vector3.new(0.03, 1.00, -0.01)
			RightGripAttachment.Parent = Handle_1

			local Script_1 = Instance.new("Script")
			Script_1.Source = "--Made by Stickmasterluke\n\n\nsp = script.Parent\n\nlocal speedboostscript = sp:WaitForChild(\'SpeedBoostScript\')\n\nfunction Equipped()\n	if sp.Parent:FindFirstChild(\'SpeedBoostScript\') == nil then\n		local s = speedboostscript:clone()\n		local tooltag = Instance.new(\'ObjectValue\')\n		tooltag.Name = \'ToolTag\'\n		tooltag.Value = sp\n		tooltag.Parent = s\n		s.Parent = sp.Parent\n		s.Disabled = false\n		local sound = sp.Handle:FindFirstChild(\'CoilSound\')\n		if sound ~= nil then\n			sound:Play()\n		end\n	end\nend\n\nsp.Equipped:connect(Equipped)"
			Script_1.Parent = SpeedCoil

			local SpeedBoostScript = Instance.new("Script")
			SpeedBoostScript.Name = "SpeedBoostScript"
			SpeedBoostScript.Source = "--Made by Stickmasterluke\n\nsp = script.Parent\n\nspeedboost = 1		--100% speed bonus\nspeedforsmoke = 10	--smoke apears when character running >= 10 studs/second.\n\nlocal tooltag = script:WaitForChild(\'ToolTag\',2)\n\nif tooltag~=nil then\n	local tool=tooltag.Value\n	local h=sp:FindFirstChild(\'Humanoid\')\n	if h~=nil then\n		h.WalkSpeed=16+16*speedboost\n		local hrp = sp:FindFirstChild(\'HumanoidRootPart\')\n		if hrp ~= nil then\n			smokepart=Instance.new(\'Part\')\n			smokepart.FormFactor=\'Custom\'\n			smokepart.Size=Vector3.new(0,0,0)\n			smokepart.TopSurface=\'Smooth\'\n			smokepart.BottomSurface=\'Smooth\'\n			smokepart.CanCollide=false\n			smokepart.Transparency=1\n			local weld=Instance.new(\'Weld\')\n			weld.Name=\'SmokePartWeld\'\n			weld.Part0 = hrp\n			weld.Part1=smokepart\n			weld.C0=CFrame.new(0,-3.5,0)*CFrame.Angles(math.pi/4,0,0)\n			weld.Parent=smokepart\n			smokepart.Parent=sp\n			smoke=Instance.new(\'Smoke\')\n			smoke.Enabled = hrp.Velocity.magnitude>speedforsmoke\n			smoke.RiseVelocity=2\n			smoke.Opacity=.25\n			smoke.Size=.5\n			smoke.Parent=smokepart\n			h.Running:connect(function(speed)\n				if smoke and smoke~=nil then\n					smoke.Enabled=speed>speedforsmoke\n				end\n			end)\n		end\n	end\n	while tool~=nil and tool.Parent==sp and h~=nil do\n		sp.ChildRemoved:wait()\n	end\n	local h=sp:FindFirstChild(\'Humanoid\')\n	if h~=nil then\n		h.WalkSpeed=game.StarterPlayer.CharacterWalkSpeed\n	end\nend\n\nif smokepart~=nil then\n	smokepart:Destroy()\nend\nscript:Destroy()\n\n\n"
			SpeedBoostScript.Parent = SpeedCoil

			local GravityCoil = Instance.new("Tool")
			GravityCoil.Name = "GravityCoil"
			GravityCoil.GripPos = Vector3.new(0.00, 0.00, 1.00)
			GravityCoil.GripRight = Vector3.new(-1.00, 0.00, 0.00)
			GravityCoil.TextureId = "http://www.roblox.com/asset/?id=16619617"
			GravityCoil.GripForward = Vector3.new(-0.00, -0.00, 1.00)
			GravityCoil.WorldPivot = CFrame.new(-109.18, 1.19, 169.57, -0.00, 0.00, 1.00)
			GravityCoil.Grip = CFrame.new(0.00, 0.00, 1.00, -0.00, -0.00, 1.00)
			GravityCoil.Parent = RobuxHandler

			local Handle_1 = Instance.new("Part")
			Handle_1.Name = "Handle"
			Handle_1.TopSurface = Enum.SurfaceType.Smooth
			Handle_1.Color = Color3.new(0.80, 0.80, 0.80)
			Handle_1.Locked = true
			Handle_1.Size = Vector3.new(1.00, 1.20, 2.00)
			Handle_1.BottomSurface = Enum.SurfaceType.Smooth
			Handle_1.Rotation = Vector3.new(180.00, 0.00, 180.00)
			Handle_1.BrickColor = BrickColor.new("Mid gray")
			Handle_1.Position = Vector3.new(-109.18, 1.19, 169.57)
			Handle_1.CFrame = CFrame.new(-109.18, 1.19, 169.57, -0.00, 0.00, 1.00)
			Handle_1.Parent = GravityCoil

			local Mesh_1 = Instance.new("SpecialMesh")
			Mesh_1.Name = "Mesh"
			Mesh_1.MeshType = Enum.MeshType.FileMesh
			Mesh_1.Scale = Vector3.new(0.70, 0.70, 0.70)
			Mesh_1.MeshId = "http://www.roblox.com/asset/?id=16606212"
			Mesh_1.TextureId = "http://www.roblox.com/asset/?id=16606141"
			Mesh_1.Parent = Handle_1

			local CoilSound_1 = Instance.new("Sound")
			CoilSound_1.Name = "CoilSound"
			CoilSound_1.Volume = 1
			CoilSound_1.SoundId = "http://www.roblox.com/asset/?id=16619553"
			CoilSound_1.Parent = Handle_1

			local RightGripAttachment_1 = Instance.new("Attachment")
			RightGripAttachment_1.Name = "RightGripAttachment"
			RightGripAttachment_1.WorldOrientation = Vector3.new(0.00, -90.00, 0.00)
			RightGripAttachment_1.CFrame = CFrame.new(0.00, 0.00, -1.00, -1.00, 0.00, -0.00)
			RightGripAttachment_1.Axis = Vector3.new(0.00, 0.00, -1.00)
			RightGripAttachment_1.WorldAxis = Vector3.new(-0.00, 0.00, 1.00)
			RightGripAttachment_1.Position = Vector3.new(0.00, 0.00, -1.00)
			RightGripAttachment_1.Orientation = Vector3.new(0.00, 90.00, 0.00)
			RightGripAttachment_1.WorldCFrame = CFrame.new(-109.18, 1.19, 170.57, 1.00, 0.00, 0.00)
			RightGripAttachment_1.WorldPosition = Vector3.new(-109.18, 1.19, 170.57)
			RightGripAttachment_1.WorldSecondaryAxis = Vector3.new(-0.00, 1.00, -0.00)
			RightGripAttachment_1.Parent = Handle_1		local Script_1 = Instance.new("Script")
			Script_1.Source = "-- Scripted by emblazes, rescripted by LucaDaBoy\n\n--// Services\nlocal Players = game:GetService(\'Players\')\n\n--// Variables\nlocal GravityCoil = script.Parent\nlocal Handle = GravityCoil.Handle\n\n\nlocal Sounds = {CoilSound = Handle.CoilSound,}\n\nlocal Gravity = 196.20\nlocal JumpHeightPercentage = 0.25\n\nlocal ToolEquipped = false\n\n--// Functions\nfunction GetAllConnectedParts(Object)\n	local Parts = {}\n	local function GetConnectedParts(Object)\n		for i, v in Object:GetConnectedParts() do\n			local Ignore = false\n			for ii, vv in Parts do\n				if v == vv then\n					Ignore = true\n				end\n			end\n			if not Ignore then\n				table.insert(Parts, v)\n				GetConnectedParts(v)\n			end\n		end\n	end\n	GetConnectedParts(Object)\n	return Parts\nend\n\nfunction SetGravityEffect()\n	if not GravityEffect or not GravityEffect.Parent then\n		GravityEffect = Instance.new(\'BodyForce\')\n		GravityEffect.Name = \'GravityCoilEffect\'\n		GravityEffect.Parent = Torso\n	end\n	\n	local TotalMass = 0\n	local ConnectedParts = GetAllConnectedParts(Torso)\n	\n	for _,v in ConnectedParts do\n		if v:IsA(\'BasePart\') then\n			TotalMass = (TotalMass + v:GetMass())\n		end\n	end\n	\n	local TotalMass = (TotalMass * 196.20 * (1 - JumpHeightPercentage))\n	GravityEffect.force = Vector3.new(0, TotalMass, 0)\nend\n\nfunction HandleGravityEffect(Enabled)\n	if not CheckIfAlive() then return end\n	\n	for _,v in Torso:GetChildren() do\n		if v:IsA(\'BodyForce\') then\n			v:Destroy()\n		end\n	end\n	\n	if not Enabled then return end\n\n	local CurrentlyEquipped = true\n	\n	GravityCoil.Unequipped:connect(function()\n		CurrentlyEquipped = false\n	end)\n	\n	SetGravityEffect()\n	\n	Character.DescendantAdded:connect(function()\n		task.wait()\n		if not CurrentlyEquipped or not CheckIfAlive() then\n			return\n		end\n		SetGravityEffect()\n	end)\n	\n	Character.DescendantRemoving:connect(function()\n		task.wait()\n		if not CurrentlyEquipped or not CheckIfAlive() then\n			return\n		end\n		SetGravityEffect()\n	end)\nend\n\nfunction CheckIfAlive()\n	return (((Character and Character.Parent and Humanoid and Humanoid.Parent and Humanoid.Health > 0 and Torso and Torso.Parent and Player and Player.Parent) and true) or false)\nend\n\nfunction Equipped(Mouse)\n	Character = GravityCoil.Parent\n	Humanoid = Character:FindFirstChild(\'Humanoid\')\n	Torso = Character:FindFirstChild(\'Torso\') or Character:FindFirstChild(\'UpperTorso\')\n	Player = Players:GetPlayerFromCharacter(Character)\n	\n	if not CheckIfAlive() then\n		return\n	end\n	if HumanoidDied then\n		HumanoidDied:Disconnect()\n	end\n	HumanoidDied = Humanoid.Died:connect(function()\n		if GravityEffect and GravityEffect.Parent then\n			GravityEffect:Destroy()\n		end\n	end)\n	Sounds.CoilSound:Play()\n	HandleGravityEffect(true)\n	ToolEquipped = true\nend\n\nfunction Unequipped()\n	if HumanoidDied then\n		HumanoidDied:Disconnect()\n	end\n	HandleGravityEffect(false)\n	ToolEquipped = false\nend\n\n--// Main\nGravityCoil.Equipped:connect(Equipped)\nGravityCoil.Unequipped:connect(Unequipped)"
			Script_1.Parent = GravityCoil

			--STARTGUI:
				local StarterGui = game:GetService("StarterGui")

			local Interface = Instance.new("ScreenGui")
			Interface.Name = "Interface"
			Interface.ResetOnSpawn = false
			Interface.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
			Interface.Parent = StarterGui

			local HUD = Instance.new("Frame")
			HUD.Name = "HUD"
			HUD.AnchorPoint = Vector2.new(0.50, 0.50)
			HUD.Size = UDim2.new(1.00, 0.00, 1.00, 0.00)
			HUD.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			HUD.Position = UDim2.new(0.50, 0.00, 0.50, 0.00)
			HUD.BorderSizePixel = 0
			HUD.BackgroundTransparency = 1
			HUD.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			HUD.Parent = Interface

			local UIAspectRatioConstraint = Instance.new("UIAspectRatioConstraint")
			UIAspectRatioConstraint.AspectRatio = 1.6299999952316284
			UIAspectRatioConstraint.Parent = HUD

			local Rebirth = Instance.new("Frame")
			Rebirth.Name = "Rebirth"
			Rebirth.Visible = false
			Rebirth.AnchorPoint = Vector2.new(0.50, 0.50)
			Rebirth.SizeConstraint = Enum.SizeConstraint.RelativeXX
			Rebirth.Size = UDim2.new(0.40, 0.00, 0.40, 0.00)
			Rebirth.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Rebirth.Position = UDim2.new(0.50, 0.00, 0.50, 0.00)
			Rebirth.BorderSizePixel = 0
			Rebirth.BackgroundTransparency = 0.30000001192092896
			Rebirth.BackgroundColor3 = Color3.new(0.08, 0.08, 0.08)
			Rebirth.Parent = HUD

			local UIAspectRatioConstraint_1 = Instance.new("UIAspectRatioConstraint")
			UIAspectRatioConstraint_1.AspectRatio = 1.5
			UIAspectRatioConstraint_1.Parent = Rebirth

			local UICorner = Instance.new("UICorner")
			UICorner.CornerRadius = UDim.new(0.04, 0.00)
			UICorner.Parent = Rebirth

			local UIStroke = Instance.new("UIStroke")
			UIStroke.Color = Color3.new(0.74, 0.74, 0.74)
			UIStroke.Thickness = 2
			UIStroke.Transparency = 0.30000001192092896
			UIStroke.Parent = Rebirth

			local Icon = Instance.new("ImageLabel")
			Icon.Name = "Icon"
			Icon.BorderSizePixel = 0
			Icon.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Icon.Image = "rbxassetid://13241715142"
			Icon.Size = UDim2.new(0.12, 0.00, 0.16, 0.00)
			Icon.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Icon.BackgroundTransparency = 1
			Icon.Position = UDim2.new(0.02, 0.00, 0.03, 0.00)
			Icon.Parent = Rebirth

			local UIAspectRatioConstraint_1 = Instance.new("UIAspectRatioConstraint")
			UIAspectRatioConstraint_1.Parent = Icon

			local Title = Instance.new("TextLabel")
			Title.Name = "Title"
			Title.TextWrapped = true
			Title.BorderSizePixel = 0
			Title.TextScaled = true
			Title.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Title.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Title.TextXAlignment = Enum.TextXAlignment.Left
			Title.TextSize = 14
			Title.Size = UDim2.new(0.40, 0.00, 0.11, 0.00)
			Title.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Title.Text = "Rebirth"
			Title.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Title.BackgroundTransparency = 1
			Title.Position = UDim2.new(0.13, 0.00, 0.05, 0.00)
			Title.Parent = Rebirth

			local Bar = Instance.new("Frame")
			Bar.Name = "Bar"
			Bar.Size = UDim2.new(0.70, 0.00, 0.01, 0.00)
			Bar.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Bar.Position = UDim2.new(0.03, 0.00, 0.19, 0.00)
			Bar.BorderSizePixel = 0
			Bar.BackgroundTransparency = 0.20000000298023224
			Bar.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Bar.Parent = Rebirth

			local UIGradient = Instance.new("UIGradient")
			UIGradient.Transparency = NumberSequence.new(NumberSequenceKeypoint.new(0.00, 0.00, 0.00), NumberSequenceKeypoint.new(0.52, 0.58, 0.00), NumberSequenceKeypoint.new(0.80, 0.49, 0.00), NumberSequenceKeypoint.new(1.00, 1.00, 0.00))
			UIGradient.Color = ColorSequence.new(ColorSequenceKeypoint.new(0.00, Color3.new(1.00, 1.00, 1.00)), ColorSequenceKeypoint.new(0.50, Color3.new(1.00, 1.00, 1.00)), ColorSequenceKeypoint.new(0.87, Color3.new(0.31, 0.31, 0.31)), ColorSequenceKeypoint.new(1.00, Color3.new(0.24, 0.24, 0.24)))
			UIGradient.Parent = Bar

			local Price = Instance.new("TextLabel")
			Price.Name = "Price"
			Price.TextWrapped = true
			Price.BorderSizePixel = 0
			Price.RichText = true
			Price.TextScaled = true
			Price.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Price.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Price.TextXAlignment = Enum.TextXAlignment.Left
			Price.TextSize = 14
			Price.Size = UDim2.new(0.97, 0.00, 0.08, 0.00)
			Price.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Price.Text = "To Rebirth you need <font color=\'rgb(15, 208, 12)\'>100K </font>💸"
			Price.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Price.BackgroundTransparency = 1
			Price.Position = UDim2.new(0.03, 0.00, 0.65, 0.00)
			Price.Parent = Rebirth

			local Description = Instance.new("TextLabel")
			Description.Name = "Description"
			Description.TextWrapped = true
			Description.BorderSizePixel = 0
			Description.RichText = true
			Description.TextScaled = true
			Description.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Description.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Description.TextXAlignment = Enum.TextXAlignment.Left
			Description.TextSize = 14
			Description.Size = UDim2.new(0.64, 0.00, 0.19, 0.00)
			Description.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Description.Text = "Rebirth to unlock more <font color=\'rgb(255,222,0)\'>buttons</font> and get a <font color=\'rgb(15, 208, 12)\'>+50% </font>💸 Boost"
			Description.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Description.BackgroundTransparency = 1
			Description.Position = UDim2.new(0.03, 0.00, 0.23, 0.00)
			Description.Parent = Rebirth

			local Buy = Instance.new("Frame")
			Buy.Name = "Buy"
			Buy.AnchorPoint = Vector2.new(0.50, 0.50)
			Buy.Size = UDim2.new(0.29, 0.00, 0.15, 0.00)
			Buy.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Buy.Position = UDim2.new(0.20, 0.00, 0.88, 0.00)
			Buy.BorderSizePixel = 0
			Buy.BackgroundTransparency = 0.30000001192092896
			Buy.BackgroundColor3 = Color3.new(0.00, 0.65, 0.97)
			Buy.Parent = Rebirth

			local UICorner_1 = Instance.new("UICorner")
			UICorner_1.CornerRadius = UDim.new(0.10, 0.00)
			UICorner_1.Parent = Buy

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Color = Color3.new(0.00, 0.33, 0.67)
			UIStroke_1.Thickness = 2
			UIStroke_1.Transparency = 0.30000001192092896
			UIStroke_1.Parent = Buy

			local Title_1 = Instance.new("TextLabel")
			Title_1.Name = "Title"
			Title_1.TextWrapped = true
			Title_1.BorderSizePixel = 0
			Title_1.TextScaled = true
			Title_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Title_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Title_1.AnchorPoint = Vector2.new(0.50, 0.50)
			Title_1.TextSize = 14
			Title_1.Size = UDim2.new(0.90, 0.00, 0.50, 0.00)
			Title_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Title_1.Text = "PURCHASE"
			Title_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Title_1.BackgroundTransparency = 1
			Title_1.Position = UDim2.new(0.50, 0.00, 0.50, 0.00)
			Title_1.Parent = Buy

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Color = Color3.new(0.00, 0.36, 0.54)
			UIStroke_1.Thickness = 2.5
			UIStroke_1.Transparency = 0.46000000834465027
			UIStroke_1.Parent = Title_1

			local UIGradient_1 = Instance.new("UIGradient")
			UIGradient_1.Color = ColorSequence.new(ColorSequenceKeypoint.new(0.00, Color3.new(1.00, 1.00, 1.00)), ColorSequenceKeypoint.new(1.00, Color3.new(0.78, 0.78, 0.78)))
			UIGradient_1.Rotation = 270
			UIGradient_1.Parent = Buy

			local Button = Instance.new("TextButton")
			Button.Name = "Button"
			Button.BorderSizePixel = 0
			Button.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Button.FontFace = Font.new("rbxasset://fonts/families/SourceSansPro.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Button.AnchorPoint = Vector2.new(0.50, 0.50)
			Button.TextSize = 14
			Button.Size = UDim2.new(1.00, 0.00, 1.00, 0.00)
			Button.TextColor3 = Color3.new(0.00, 0.00, 0.00)
			Button.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Button.Text = ""
			Button.BackgroundTransparency = 1
			Button.Position = UDim2.new(0.50, 0.00, 0.50, 0.00)
			Button.Parent = Buy

			local Multi = Instance.new("TextLabel")
			Multi.Name = "Multi"
			Multi.TextWrapped = true
			Multi.BorderSizePixel = 0
			Multi.RichText = true
			Multi.TextScaled = true
			Multi.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Multi.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Multi.TextXAlignment = Enum.TextXAlignment.Left
			Multi.TextSize = 14
			Multi.Size = UDim2.new(0.97, 0.00, 0.08, 0.00)
			Multi.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Multi.Text = "Current Multiplier:  <font color=\'rgb(15, 208, 12)\'>x1.5 </font>💸"
			Multi.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Multi.BackgroundTransparency = 1
			Multi.Position = UDim2.new(0.03, 0.00, 0.47, 0.00)
			Multi.Parent = Rebirth

			local UIGradient_1 = Instance.new("UIGradient")
			UIGradient_1.Color = ColorSequence.new(ColorSequenceKeypoint.new(0.00, Color3.new(1.00, 1.00, 1.00)), ColorSequenceKeypoint.new(1.00, Color3.new(0.00, 0.00, 0.00)))
			UIGradient_1.Rotation = 90
			UIGradient_1.Parent = Rebirth

			local Close = Instance.new("Frame")
			Close.Name = "Close"
			Close.AnchorPoint = Vector2.new(1.00, 0.00)
			Close.Size = UDim2.new(0.08, 0.00, 0.13, 0.00)
			Close.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Close.Position = UDim2.new(0.98, 0.00, 0.03, 0.00)
			Close.BorderSizePixel = 0
			Close.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Close.Parent = Rebirth

			local UICorner_1 = Instance.new("UICorner")
			UICorner_1.CornerRadius = UDim.new(0.20, 0.00)
			UICorner_1.Parent = Close

			local UIGradient_1 = Instance.new("UIGradient")
			UIGradient_1.Color = ColorSequence.new(ColorSequenceKeypoint.new(0.00, Color3.new(0.47, 0.18, 0.18)), ColorSequenceKeypoint.new(1.00, Color3.new(1.00, 0.22, 0.22)))
			UIGradient_1.Rotation = 90
			UIGradient_1.Parent = Close

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Color = Color3.new(1.00, 1.00, 1.00)
			UIStroke_1.Thickness = 1.7999999523162842
			UIStroke_1.Transparency = 0.6499999761581421
			UIStroke_1.Parent = Close

			local TextLabel = Instance.new("TextLabel")
			TextLabel.TextWrapped = true
			TextLabel.BorderSizePixel = 0
			TextLabel.TextScaled = true
			TextLabel.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			TextLabel.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			TextLabel.TextSize = 14
			TextLabel.Size = UDim2.new(0.71, 0.00, 0.72, 0.00)
			TextLabel.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			TextLabel.Text = "X"
			TextLabel.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			TextLabel.BackgroundTransparency = 1
			TextLabel.Position = UDim2.new(0.14, 0.00, 0.15, 0.00)
			TextLabel.Parent = Close

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Color = Color3.new(0.36, 0.11, 0.11)
			UIStroke_1.Thickness = 2.5
			UIStroke_1.Transparency = 0.46000000834465027
			UIStroke_1.Parent = TextLabel

			local UIAspectRatioConstraint_1 = Instance.new("UIAspectRatioConstraint")
			UIAspectRatioConstraint_1.Parent = Close

			local Button_1 = Instance.new("TextButton")
			Button_1.Name = "Button"
			Button_1.BorderSizePixel = 0
			Button_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Button_1.FontFace = Font.new("rbxasset://fonts/families/SourceSansPro.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Button_1.AnchorPoint = Vector2.new(0.50, 0.50)
			Button_1.TextSize = 14
			Button_1.Size = UDim2.new(1.00, 0.00, 1.00, 0.00)
			Button_1.TextColor3 = Color3.new(0.00, 0.00, 0.00)
			Button_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Button_1.Text = ""
			Button_1.BackgroundTransparency = 1
			Button_1.Position = UDim2.new(0.50, 0.00, 0.50, 0.00)
			Button_1.Parent = Close

			local Shop = Instance.new("Frame")
			Shop.Name = "Shop"
			Shop.Visible = false
			Shop.AnchorPoint = Vector2.new(0.50, 0.50)
			Shop.Size = UDim2.new(0.51, 0.00, 0.58, 0.00)
			Shop.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Shop.Position = UDim2.new(0.50, 0.00, 0.50, 0.00)
			Shop.BorderSizePixel = 0
			Shop.BackgroundTransparency = 0.30000001192092896
			Shop.BackgroundColor3 = Color3.new(0.08, 0.08, 0.08)
			Shop.Parent = HUD

			local ObjectHolder = Instance.new("ScrollingFrame")
			ObjectHolder.Name = "ObjectHolder"
			ObjectHolder.Active = true
			ObjectHolder.ScrollingDirection = Enum.ScrollingDirection.Y
			ObjectHolder.BorderSizePixel = 0
			ObjectHolder.AutomaticCanvasSize = Enum.AutomaticSize.Y
			ObjectHolder.AnchorPoint = Vector2.new(0.50, 0.50)
			ObjectHolder.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			ObjectHolder.Size = UDim2.new(0.96, 0.00, 0.80, 0.00)
			ObjectHolder.ScrollBarImageColor3 = Color3.new(0.00, 0.00, 0.00)
			ObjectHolder.ScrollBarThickness = 4
			ObjectHolder.BackgroundTransparency = 1
			ObjectHolder.Position = UDim2.new(0.50, 0.00, 0.57, 0.00)
			ObjectHolder.Parent = Shop

			local UIListLayout = Instance.new("UIListLayout")
			UIListLayout.Padding = UDim.new(0.00, 10.00)
			UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder
			UIListLayout.Parent = ObjectHolder

			local GamepassFrame = Instance.new("Frame")
			GamepassFrame.Name = "GamepassFrame"
			GamepassFrame.AnchorPoint = Vector2.new(0.50, 0.50)
			GamepassFrame.Size = UDim2.new(1.00, 0.00, 0.34, 0.00)
			GamepassFrame.Position = UDim2.new(0.50, 0.00, 0.17, 0.00)
			GamepassFrame.BorderSizePixel = 0
			GamepassFrame.BackgroundTransparency = 0.800000011920929
			GamepassFrame.BackgroundColor3 = Color3.new(0.87, 0.87, 0.84)
			GamepassFrame.Parent = ObjectHolder

			local Icon_1 = Instance.new("ImageLabel")
			Icon_1.Name = "Icon"
			Icon_1.BorderSizePixel = 0
			Icon_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Icon_1.AnchorPoint = Vector2.new(0.50, 0.50)
			Icon_1.Image = "rbxasset://textures/ui/GuiImagePlaceholder.png"
			Icon_1.Size = UDim2.new(0.15, 0.00, 0.89, 0.00)
			Icon_1.BackgroundTransparency = 1
			Icon_1.Position = UDim2.new(0.09, 0.00, 0.50, 0.00)
			Icon_1.Parent = GamepassFrame

			local Title_1 = Instance.new("TextLabel")
			Title_1.Name = "Title"
			Title_1.TextWrapped = true
			Title_1.BorderSizePixel = 0
			Title_1.TextYAlignment = Enum.TextYAlignment.Top
			Title_1.TextScaled = true
			Title_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Title_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Title_1.AnchorPoint = Vector2.new(0.50, 0.50)
			Title_1.TextXAlignment = Enum.TextXAlignment.Left
			Title_1.TextSize = 14
			Title_1.Size = UDim2.new(0.59, 0.00, 0.21, 0.00)
			Title_1.Text = "Gamepass Name"
			Title_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Title_1.BackgroundTransparency = 1
			Title_1.Position = UDim2.new(0.47, 0.00, 0.16, 0.00)
			Title_1.Parent = GamepassFrame

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 3
			UIStroke_1.Parent = Title_1		
			local Description_1 = Instance.new("TextLabel")
			Description_1.Name = "Description"
			Description_1.TextWrapped = true
			Description_1.BorderSizePixel = 0
			Description_1.TextYAlignment = Enum.TextYAlignment.Top
			Description_1.TextScaled = true
			Description_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Description_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Description_1.AnchorPoint = Vector2.new(0.50, 0.50)
			Description_1.TextXAlignment = Enum.TextXAlignment.Left
			Description_1.TextSize = 14
			Description_1.Size = UDim2.new(0.49, 0.00, 0.68, 0.00)
			Description_1.Text = "Gamepass description."
			Description_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Description_1.BackgroundTransparency = 1
			Description_1.Position = UDim2.new(0.42, 0.00, 0.60, 0.00)
			Description_1.Parent = GamepassFrame

			local UITextSizeConstraint = Instance.new("UITextSizeConstraint")
			UITextSizeConstraint.MaxTextSize = 20
			UITextSizeConstraint.Parent = Description_1

			local BuyButton = Instance.new("TextButton")
			BuyButton.Name = "BuyButton"
			BuyButton.TextWrapped = true
			BuyButton.BorderSizePixel = 0
			BuyButton.TextScaled = true
			BuyButton.BackgroundColor3 = Color3.new(0.00, 0.94, 0.30)
			BuyButton.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			BuyButton.AnchorPoint = Vector2.new(0.50, 0.50)
			BuyButton.TextSize = 14
			BuyButton.Size = UDim2.new(0.29, 0.00, 0.42, 0.00)
			BuyButton.TextColor3 = Color3.new(0.96, 0.96, 0.91)
			BuyButton.Text = "BUY"
			BuyButton.Position = UDim2.new(0.84, 0.00, 0.54, 0.00)
			BuyButton.Parent = GamepassFrame

			local UICorner_1 = Instance.new("UICorner")
			UICorner_1.CornerRadius = UDim.new(0.00, 10.00)
			UICorner_1.Parent = BuyButton

			local UIStroke1 = Instance.new("UIStroke")
			UIStroke1.Name = "UIStroke1"
			UIStroke1.ApplyStrokeMode = Enum.ApplyStrokeMode.Border
			UIStroke1.Thickness = 4
			UIStroke1.Parent = BuyButton

			local UIStroke2 = Instance.new("UIStroke")
			UIStroke2.Name = "UIStroke2"
			UIStroke2.Thickness = 2
			UIStroke2.Parent = BuyButton

			local UICorner_1 = Instance.new("UICorner")
			UICorner_1.CornerRadius = UDim.new(0.00, 10.00)
			UICorner_1.Parent = GamepassFrame

			local Price_1 = Instance.new("TextLabel")
			Price_1.Name = "Price"
			Price_1.TextWrapped = true
			Price_1.BorderSizePixel = 0
			Price_1.TextScaled = true
			Price_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Price_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Price_1.AnchorPoint = Vector2.new(0.50, 0.50)
			Price_1.TextSize = 14
			Price_1.Size = UDim2.new(0.26, 0.00, 0.20, 0.00)
			Price_1.Text = "500 Robux"
			Price_1.TextColor3 = Color3.new(0.00, 0.94, 0.30)
			Price_1.BackgroundTransparency = 1
			Price_1.Position = UDim2.new(0.84, 0.00, 0.16, 0.00)
			Price_1.Parent = GamepassFrame

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Thickness = 2
			UIStroke_1.Parent = Price_1

			local UIAspectRatioConstraint_1 = Instance.new("UIAspectRatioConstraint")
			UIAspectRatioConstraint_1.AspectRatio = 5.550724506378174
			UIAspectRatioConstraint_1.Parent = GamepassFrame

			local UIAspectRatioConstraint_1 = Instance.new("UIAspectRatioConstraint")
			UIAspectRatioConstraint_1.AspectRatio = 1.57905113697052
			UIAspectRatioConstraint_1.Parent = Shop

			local Close_1 = Instance.new("Frame")
			Close_1.Name = "Close"
			Close_1.AnchorPoint = Vector2.new(1.00, 0.00)
			Close_1.Size = UDim2.new(0.08, 0.00, 0.13, 0.00)
			Close_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Close_1.Position = UDim2.new(0.99, 0.00, 0.03, 0.00)
			Close_1.BorderSizePixel = 0
			Close_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Close_1.Parent = Shop

			local UICorner_1 = Instance.new("UICorner")
			UICorner_1.CornerRadius = UDim.new(0.20, 0.00)
			UICorner_1.Parent = Close_1

			local UIGradient_1 = Instance.new("UIGradient")
			UIGradient_1.Color = ColorSequence.new(ColorSequenceKeypoint.new(0.00, Color3.new(0.47, 0.18, 0.18)), ColorSequenceKeypoint.new(1.00, Color3.new(1.00, 0.22, 0.22)))
			UIGradient_1.Rotation = 90
			UIGradient_1.Parent = Close_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Color = Color3.new(1.00, 1.00, 1.00)
			UIStroke_1.Thickness = 1.7999999523162842
			UIStroke_1.Transparency = 0.6499999761581421
			UIStroke_1.Parent = Close_1

			local TextLabel_1 = Instance.new("TextLabel")
			TextLabel_1.TextWrapped = true
			TextLabel_1.BorderSizePixel = 0
			TextLabel_1.TextScaled = true
			TextLabel_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			TextLabel_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			TextLabel_1.TextSize = 14
			TextLabel_1.Size = UDim2.new(0.71, 0.00, 0.72, 0.00)
			TextLabel_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			TextLabel_1.Text = "X"
			TextLabel_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			TextLabel_1.BackgroundTransparency = 1
			TextLabel_1.Position = UDim2.new(0.14, 0.00, 0.15, 0.00)
			TextLabel_1.Parent = Close_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Color = Color3.new(0.36, 0.11, 0.11)
			UIStroke_1.Thickness = 2.5
			UIStroke_1.Transparency = 0.46000000834465027
			UIStroke_1.Parent = TextLabel_1

			local UIAspectRatioConstraint_1 = Instance.new("UIAspectRatioConstraint")
			UIAspectRatioConstraint_1.Parent = Close_1

			local Button_1 = Instance.new("TextButton")
			Button_1.Name = "Button"
			Button_1.BorderSizePixel = 0
			Button_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Button_1.FontFace = Font.new("rbxasset://fonts/families/SourceSansPro.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Button_1.AnchorPoint = Vector2.new(0.50, 0.50)
			Button_1.TextSize = 14
			Button_1.Size = UDim2.new(1.00, 0.00, 1.00, 0.00)
			Button_1.TextColor3 = Color3.new(0.00, 0.00, 0.00)
			Button_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Button_1.Text = ""
			Button_1.BackgroundTransparency = 1
			Button_1.Position = UDim2.new(0.50, 0.00, 0.50, 0.00)
			Button_1.Parent = Close_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Color = Color3.new(0.74, 0.74, 0.74)
			UIStroke_1.Thickness = 2
			UIStroke_1.Transparency = 0.30000001192092896
			UIStroke_1.Parent = Shop

			local Title_1 = Instance.new("TextLabel")
			Title_1.Name = "Title"
			Title_1.TextWrapped = true
			Title_1.BorderSizePixel = 0
			Title_1.TextScaled = true
			Title_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Title_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Title_1.TextXAlignment = Enum.TextXAlignment.Left
			Title_1.TextSize = 14
			Title_1.Size = UDim2.new(0.55, 0.00, 0.17, 0.00)
			Title_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Title_1.Text = "Gamepass Shop"
			Title_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Title_1.BackgroundTransparency = 1
			Title_1.Position = UDim2.new(0.03, 0.00, -0.00, 0.00)
			Title_1.Parent = Shop

			local UICorner_1 = Instance.new("UICorner")
			UICorner_1.CornerRadius = UDim.new(0.00, 30.00)
			UICorner_1.Parent = Title_1

			local Bar_1 = Instance.new("Frame")
			Bar_1.Name = "Bar"
			Bar_1.Size = UDim2.new(0.70, 0.00, 0.01, 0.00)
			Bar_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Bar_1.Position = UDim2.new(0.04, 0.00, 0.15, 0.00)
			Bar_1.BorderSizePixel = 0
			Bar_1.BackgroundTransparency = 0.20000000298023224
			Bar_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Bar_1.Parent = Shop

			local UIGradient_1 = Instance.new("UIGradient")
			UIGradient_1.Transparency = NumberSequence.new(NumberSequenceKeypoint.new(0.00, 0.00, 0.00), NumberSequenceKeypoint.new(0.52, 0.58, 0.00), NumberSequenceKeypoint.new(0.80, 0.49, 0.00), NumberSequenceKeypoint.new(1.00, 1.00, 0.00))
			UIGradient_1.Color = ColorSequence.new(ColorSequenceKeypoint.new(0.00, Color3.new(1.00, 1.00, 1.00)), ColorSequenceKeypoint.new(0.50, Color3.new(1.00, 1.00, 1.00)), ColorSequenceKeypoint.new(0.87, Color3.new(0.31, 0.31, 0.31)), ColorSequenceKeypoint.new(1.00, Color3.new(0.24, 0.24, 0.24)))
			UIGradient_1.Parent = Bar_1

			local UICorner_1 = Instance.new("UICorner")
			UICorner_1.CornerRadius = UDim.new(0.04, 0.00)
			UICorner_1.Parent = Shop

			local MoneyLabel = Instance.new("Frame")
			MoneyLabel.Name = "MoneyLabel"
			MoneyLabel.Size = UDim2.new(0.21, 0.00, 0.07, 0.00)
			MoneyLabel.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			MoneyLabel.Position = UDim2.new(0.39, 0.00, 0.03, 0.00)
			MoneyLabel.BorderSizePixel = 0
			MoneyLabel.BackgroundTransparency = 0.30000001192092896
			MoneyLabel.BackgroundColor3 = Color3.new(0.08, 0.08, 0.08)
			MoneyLabel.Parent = HUD

			local Main = Instance.new("TextLabel")
			Main.Name = "Main"
			Main.TextWrapped = true
			Main.ZIndex = 3
			Main.BorderSizePixel = 0
			Main.TextScaled = true
			Main.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Main.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Medium, Enum.FontStyle.Normal)
			Main.TextXAlignment = Enum.TextXAlignment.Left
			Main.TextSize = 10
			Main.Size = UDim2.new(0.68, 0.00, 0.86, 0.00)
			Main.Text = "$0"
			Main.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Main.BackgroundTransparency = 1
			Main.Position = UDim2.new(0.26, 0.00, 0.05, 0.00)
			Main.Parent = MoneyLabel

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Color = Color3.new(0.05, 0.05, 0.05)
			UIStroke_1.Thickness = 2
			UIStroke_1.Transparency = 0.30000001192092896
			UIStroke_1.Parent = Main

			local Coin = Instance.new("ImageLabel")
			Coin.Name = "Coin"
			Coin.ZIndex = 5
			Coin.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Coin.AnchorPoint = Vector2.new(0.00, 0.50)
			Coin.Image = "rbxassetid://15446457340"
			Coin.Size = UDim2.new(0.23, 0.00, 0.88, 0.00)
			Coin.BackgroundTransparency = 1
			Coin.Position = UDim2.new(0.06, 0.00, 0.50, 0.00)
			Coin.Parent = MoneyLabel

			local UIAspectRatioConstraint_1 = Instance.new("UIAspectRatioConstraint")
			UIAspectRatioConstraint_1.Parent = Coin

			local UICorner_1 = Instance.new("UICorner")
			UICorner_1.CornerRadius = UDim.new(1.00, 0.00)
			UICorner_1.Parent = MoneyLabel

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Color = Color3.new(0.74, 0.74, 0.74)
			UIStroke_1.Thickness = 2
			UIStroke_1.Transparency = 0.30000001192092896
			UIStroke_1.Parent = MoneyLabel

			local Leftside = Instance.new("Frame")
			Leftside.Name = "Leftside"
			Leftside.AnchorPoint = Vector2.new(0.00, 0.50)
			Leftside.Size = UDim2.new(0.18, 0.00, 0.40, 0.00)
			Leftside.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Leftside.Position = UDim2.new(0.00, 0.00, 0.50, 0.00)
			Leftside.BorderSizePixel = 0
			Leftside.BackgroundTransparency = 1
			Leftside.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Leftside.Parent = Interface

			local UIAspectRatioConstraint_1 = Instance.new("UIAspectRatioConstraint")
			UIAspectRatioConstraint_1.AspectRatio = 0.6700000166893005
			UIAspectRatioConstraint_1.Parent = Leftside

			local RebirthBT = Instance.new("Frame")
			RebirthBT.Name = "RebirthBT"
			RebirthBT.AnchorPoint = Vector2.new(0.50, 0.50)
			RebirthBT.SizeConstraint = Enum.SizeConstraint.RelativeXX
			RebirthBT.Size = UDim2.new(0.45, 0.00, 0.50, 0.00)
			RebirthBT.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			RebirthBT.Position = UDim2.new(0.32, 0.00, 0.40, 0.00)
			RebirthBT.BorderSizePixel = 0
			RebirthBT.BackgroundTransparency = 0.30000001192092896
			RebirthBT.BackgroundColor3 = Color3.new(0.08, 0.08, 0.08)
			RebirthBT.Parent = Leftside

			local UIAspectRatioConstraint_1 = Instance.new("UIAspectRatioConstraint")
			UIAspectRatioConstraint_1.Parent = RebirthBT

			local UICorner_1 = Instance.new("UICorner")
			UICorner_1.CornerRadius = UDim.new(0.18, 0.00)
			UICorner_1.Parent = RebirthBT

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Color = Color3.new(0.74, 0.74, 0.74)
			UIStroke_1.Thickness = 2
			UIStroke_1.Transparency = 0.30000001192092896
			UIStroke_1.Parent = RebirthBT

			local Icon_1 = Instance.new("ImageLabel")
			Icon_1.Name = "Icon"
			Icon_1.Active = true
			Icon_1.BorderSizePixel = 0
			Icon_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Icon_1.AnchorPoint = Vector2.new(0.50, 0.50)
			Icon_1.Image = "rbxassetid://13241715142"
			Icon_1.Size = UDim2.new(0.90, 0.00, 0.90, 0.00)
			Icon_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Icon_1.BackgroundTransparency = 1
			Icon_1.Position = UDim2.new(0.50, 0.00, 0.50, 0.00)
			Icon_1.Parent = RebirthBT

			local UIAspectRatioConstraint_1 = Instance.new("UIAspectRatioConstraint")
			UIAspectRatioConstraint_1.Parent = Icon_1

			local Title_1 = Instance.new("TextLabel")
			Title_1.Name = "Title"
			Title_1.TextWrapped = true
			Title_1.BorderSizePixel = 0
			Title_1.TextScaled = true
			Title_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Title_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Title_1.AnchorPoint = Vector2.new(0.50, 0.50)
			Title_1.TextSize = 14
			Title_1.Size = UDim2.new(0.85, 0.00, 0.90, 0.00)
			Title_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Title_1.Text = "Rebirth"
			Title_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Title_1.BackgroundTransparency = 1
			Title_1.Position = UDim2.new(0.50, 0.00, 0.50, 0.00)
			Title_1.Parent = RebirthBT

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Color = Color3.new(0.05, 0.05, 0.05)
			UIStroke_1.Thickness = 2
			UIStroke_1.Transparency = 0.30000001192092896
			UIStroke_1.Parent = Title_1

			local UIGradient_1 = Instance.new("UIGradient")
			UIGradient_1.Color = ColorSequence.new(ColorSequenceKeypoint.new(0.00, Color3.new(1.00, 1.00, 1.00)), ColorSequenceKeypoint.new(1.00, Color3.new(0.00, 0.00, 0.00)))
			UIGradient_1.Rotation = 90
			UIGradient_1.Parent = RebirthBT

			local Notification = Instance.new("Frame")
			Notification.Name = "Notification"
			Notification.Visible = false
			Notification.AnchorPoint = Vector2.new(1.00, 0.00)
			Notification.Size = UDim2.new(0.25, 0.00, 0.25, 0.00)
			Notification.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Notification.Position = UDim2.new(1.10, 0.00, -0.05, 0.00)
			Notification.BorderSizePixel = 0
			Notification.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Notification.Parent = RebirthBT

			local UIAspectRatioConstraint_1 = Instance.new("UIAspectRatioConstraint")
			UIAspectRatioConstraint_1.Parent = Notification

			local UICorner_1 = Instance.new("UICorner")
			UICorner_1.CornerRadius = UDim.new(0.50, 0.00)
			UICorner_1.Parent = Notification

			local Title_1 = Instance.new("TextLabel")
			Title_1.Name = "Title"
			Title_1.TextWrapped = true
			Title_1.BorderSizePixel = 0
			Title_1.TextScaled = true
			Title_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Title_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Title_1.AnchorPoint = Vector2.new(0.50, 0.50)
			Title_1.TextSize = 14
			Title_1.Size = UDim2.new(0.85, 0.00, 0.90, 0.00)
			Title_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Title_1.Text = "!"
			Title_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Title_1.BackgroundTransparency = 1
			Title_1.Position = UDim2.new(0.50, 0.00, 0.50, 0.00)
			Title_1.Parent = Notification

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Color = Color3.new(0.37, 0.00, 0.00)
			UIStroke_1.Thickness = 2
			UIStroke_1.Transparency = 0.30000001192092896
			UIStroke_1.Parent = Notification

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Color = Color3.new(1.00, 1.00, 1.00)
			UIStroke_1.Thickness = 1.7999999523162842
			UIStroke_1.Transparency = 0.6499999761581421
			UIStroke_1.Parent = Notification
			local UIGradient_1 = Instance.new("UIGradient")
			UIGradient_1.Color = ColorSequence.new(ColorSequenceKeypoint.new(0.00, Color3.new(0.55, 0.21, 0.21)), ColorSequenceKeypoint.new(1.00, Color3.new(1.00, 0.22, 0.22)))
			UIGradient_1.Rotation = 90
			UIGradient_1.Parent = Notification

			local Button_1 = Instance.new("TextButton")
			Button_1.Name = "Button"
			Button_1.BorderSizePixel = 0
			Button_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Button_1.FontFace = Font.new("rbxasset://fonts/families/SourceSansPro.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Button_1.AnchorPoint = Vector2.new(0.50, 0.50)
			Button_1.TextSize = 14
			Button_1.Size = UDim2.new(1.00, 0.00, 1.00, 0.00)
			Button_1.TextColor3 = Color3.new(0.00, 0.00, 0.00)
			Button_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Button_1.Text = ""
			Button_1.BackgroundTransparency = 1
			Button_1.Position = UDim2.new(0.50, 0.00, 0.50, 0.00)
			Button_1.Parent = RebirthBT

			local ShopBT = Instance.new("Frame")
			ShopBT.Name = "ShopBT"
			ShopBT.AnchorPoint = Vector2.new(0.50, 0.50)
			ShopBT.SizeConstraint = Enum.SizeConstraint.RelativeXX
			ShopBT.Size = UDim2.new(0.45, 0.00, 0.50, 0.00)
			ShopBT.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			ShopBT.Position = UDim2.new(0.32, 0.00, 0.77, 0.00)
			ShopBT.BorderSizePixel = 0
			ShopBT.BackgroundTransparency = 0.30000001192092896
			ShopBT.BackgroundColor3 = Color3.new(0.08, 0.08, 0.08)
			ShopBT.Parent = Leftside

			local UIAspectRatioConstraint_1 = Instance.new("UIAspectRatioConstraint")
			UIAspectRatioConstraint_1.Parent = ShopBT

			local UICorner_1 = Instance.new("UICorner")
			UICorner_1.CornerRadius = UDim.new(0.18, 0.00)
			UICorner_1.Parent = ShopBT

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Color = Color3.new(0.74, 0.74, 0.74)
			UIStroke_1.Thickness = 2
			UIStroke_1.Transparency = 0.30000001192092896
			UIStroke_1.Parent = ShopBT

			local Icon_1 = Instance.new("ImageLabel")
			Icon_1.Name = "Icon"
			Icon_1.Active = true
			Icon_1.BorderSizePixel = 0
			Icon_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Icon_1.AnchorPoint = Vector2.new(0.50, 0.50)
			Icon_1.Image = "rbxassetid://18343980587"
			Icon_1.Size = UDim2.new(0.90, 0.00, 0.90, 0.00)
			Icon_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Icon_1.BackgroundTransparency = 1
			Icon_1.Position = UDim2.new(0.50, 0.00, 0.50, 0.00)
			Icon_1.Parent = ShopBT

			local UIAspectRatioConstraint_1 = Instance.new("UIAspectRatioConstraint")
			UIAspectRatioConstraint_1.Parent = Icon_1

			local Title_1 = Instance.new("TextLabel")
			Title_1.Name = "Title"
			Title_1.TextWrapped = true
			Title_1.BorderSizePixel = 0
			Title_1.TextScaled = true
			Title_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Title_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Title_1.AnchorPoint = Vector2.new(0.50, 0.50)
			Title_1.TextSize = 14
			Title_1.Size = UDim2.new(0.85, 0.00, 0.35, 0.00)
			Title_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Title_1.Text = "Shop"
			Title_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Title_1.BackgroundTransparency = 1
			Title_1.Position = UDim2.new(0.50, 0.00, 0.55, 0.00)
			Title_1.Parent = ShopBT

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Color = Color3.new(0.05, 0.05, 0.05)
			UIStroke_1.Thickness = 2
			UIStroke_1.Transparency = 0.30000001192092896
			UIStroke_1.Parent = Title_1

			local UIGradient_1 = Instance.new("UIGradient")
			UIGradient_1.Color = ColorSequence.new(ColorSequenceKeypoint.new(0.00, Color3.new(1.00, 1.00, 1.00)), ColorSequenceKeypoint.new(1.00, Color3.new(0.00, 0.00, 0.00)))
			UIGradient_1.Rotation = 90
			UIGradient_1.Parent = ShopBT

			local Notification_1 = Instance.new("Frame")
			Notification_1.Name = "Notification"
			Notification_1.Visible = false
			Notification_1.AnchorPoint = Vector2.new(1.00, 0.00)
			Notification_1.Size = UDim2.new(0.25, 0.00, 0.25, 0.00)
			Notification_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Notification_1.Position = UDim2.new(1.10, 0.00, -0.05, 0.00)
			Notification_1.BorderSizePixel = 0
			Notification_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Notification_1.Parent = ShopBT

			local UIAspectRatioConstraint_1 = Instance.new("UIAspectRatioConstraint")
			UIAspectRatioConstraint_1.Parent = Notification_1

			local UICorner_1 = Instance.new("UICorner")
			UICorner_1.CornerRadius = UDim.new(0.50, 0.00)
			UICorner_1.Parent = Notification_1

			local Title_1 = Instance.new("TextLabel")
			Title_1.Name = "Title"
			Title_1.TextWrapped = true
			Title_1.BorderSizePixel = 0
			Title_1.TextScaled = true
			Title_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Title_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Title_1.AnchorPoint = Vector2.new(0.50, 0.50)
			Title_1.TextSize = 14
			Title_1.Size = UDim2.new(0.85, 0.00, 0.90, 0.00)
			Title_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Title_1.Text = "!"
			Title_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
			Title_1.BackgroundTransparency = 1
			Title_1.Position = UDim2.new(0.50, 0.00, 0.50, 0.00)
			Title_1.Parent = Notification_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Color = Color3.new(0.37, 0.00, 0.00)
			UIStroke_1.Thickness = 2
			UIStroke_1.Transparency = 0.30000001192092896
			UIStroke_1.Parent = Notification_1

			local UIStroke_1 = Instance.new("UIStroke")
			UIStroke_1.Color = Color3.new(1.00, 1.00, 1.00)
			UIStroke_1.Thickness = 1.7999999523162842
			UIStroke_1.Transparency = 0.6499999761581421
			UIStroke_1.Parent = Notification_1

			local UIGradient_1 = Instance.new("UIGradient")
			UIGradient_1.Color = ColorSequence.new(ColorSequenceKeypoint.new(0.00, Color3.new(0.55, 0.21, 0.21)), ColorSequenceKeypoint.new(1.00, Color3.new(1.00, 0.22, 0.22)))
			UIGradient_1.Rotation = 90
			UIGradient_1.Parent = Notification_1

			local Button_1 = Instance.new("TextButton")
			Button_1.Name = "Button"
			Button_1.BorderSizePixel = 0
			Button_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
			Button_1.FontFace = Font.new("rbxasset://fonts/families/SourceSansPro.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
			Button_1.AnchorPoint = Vector2.new(0.50, 0.50)
			Button_1.TextSize = 14
			Button_1.Size = UDim2.new(1.00, 0.00, 1.00, 0.00)
			Button_1.TextColor3 = Color3.new(0.00, 0.00, 0.00)
			Button_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
			Button_1.Text = ""
			Button_1.BackgroundTransparency = 1
			Button_1.Position = UDim2.new(0.50, 0.00, 0.50, 0.00)
			Button_1.Parent = ShopBT
   	local UIGradient_1 = Instance.new("UIGradient")
	UIGradient_1.Color = ColorSequence.new(ColorSequenceKeypoint.new(0.00, Color3.new(0.55, 0.21, 0.21)), ColorSequenceKeypoint.new(1.00, Color3.new(1.00, 0.22, 0.22)))
	UIGradient_1.Rotation = 90
	UIGradient_1.Parent = Notification
	
	local Button_1 = Instance.new("TextButton")
	Button_1.Name = "Button"
	Button_1.BorderSizePixel = 0
	Button_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	Button_1.FontFace = Font.new("rbxasset://fonts/families/SourceSansPro.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
	Button_1.AnchorPoint = Vector2.new(0.50, 0.50)
	Button_1.TextSize = 14
	Button_1.Size = UDim2.new(1.00, 0.00, 1.00, 0.00)
	Button_1.TextColor3 = Color3.new(0.00, 0.00, 0.00)
	Button_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Button_1.Text = ""
	Button_1.BackgroundTransparency = 1
	Button_1.Position = UDim2.new(0.50, 0.00, 0.50, 0.00)
	Button_1.Parent = RebirthBT
	
	local ShopBT = Instance.new("Frame")
	ShopBT.Name = "ShopBT"
	ShopBT.AnchorPoint = Vector2.new(0.50, 0.50)
	ShopBT.SizeConstraint = Enum.SizeConstraint.RelativeXX
	ShopBT.Size = UDim2.new(0.45, 0.00, 0.50, 0.00)
	ShopBT.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	ShopBT.Position = UDim2.new(0.32, 0.00, 0.77, 0.00)
	ShopBT.BorderSizePixel = 0
	ShopBT.BackgroundTransparency = 0.30000001192092896
	ShopBT.BackgroundColor3 = Color3.new(0.08, 0.08, 0.08)
	ShopBT.Parent = Leftside
	
	local UIAspectRatioConstraint_1 = Instance.new("UIAspectRatioConstraint")
	UIAspectRatioConstraint_1.Parent = ShopBT
	
	local UICorner_1 = Instance.new("UICorner")
	UICorner_1.CornerRadius = UDim.new(0.18, 0.00)
	UICorner_1.Parent = ShopBT
	
	local UIStroke_1 = Instance.new("UIStroke")
	UIStroke_1.Color = Color3.new(0.74, 0.74, 0.74)
	UIStroke_1.Thickness = 2
	UIStroke_1.Transparency = 0.30000001192092896
	UIStroke_1.Parent = ShopBT
	
	local Icon_1 = Instance.new("ImageLabel")
	Icon_1.Name = "Icon"
	Icon_1.Active = true
	Icon_1.BorderSizePixel = 0
	Icon_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	Icon_1.AnchorPoint = Vector2.new(0.50, 0.50)
	Icon_1.Image = "rbxassetid://18343980587"
	Icon_1.Size = UDim2.new(0.90, 0.00, 0.90, 0.00)
	Icon_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Icon_1.BackgroundTransparency = 1
	Icon_1.Position = UDim2.new(0.50, 0.00, 0.50, 0.00)
	Icon_1.Parent = ShopBT
	
	local UIAspectRatioConstraint_1 = Instance.new("UIAspectRatioConstraint")
	UIAspectRatioConstraint_1.Parent = Icon_1
	
	local Title_1 = Instance.new("TextLabel")
	Title_1.Name = "Title"
	Title_1.TextWrapped = true
	Title_1.BorderSizePixel = 0
	Title_1.TextScaled = true
	Title_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	Title_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
	Title_1.AnchorPoint = Vector2.new(0.50, 0.50)
	Title_1.TextSize = 14
	Title_1.Size = UDim2.new(0.85, 0.00, 0.35, 0.00)
	Title_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Title_1.Text = "Shop"
	Title_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
	Title_1.BackgroundTransparency = 1
	Title_1.Position = UDim2.new(0.50, 0.00, 0.55, 0.00)
	Title_1.Parent = ShopBT
	
	local UIStroke_1 = Instance.new("UIStroke")
	UIStroke_1.Color = Color3.new(0.05, 0.05, 0.05)
	UIStroke_1.Thickness = 2
	UIStroke_1.Transparency = 0.30000001192092896
	UIStroke_1.Parent = Title_1
	
	local UIGradient_1 = Instance.new("UIGradient")
	UIGradient_1.Color = ColorSequence.new(ColorSequenceKeypoint.new(0.00, Color3.new(1.00, 1.00, 1.00)), ColorSequenceKeypoint.new(1.00, Color3.new(0.00, 0.00, 0.00)))
	UIGradient_1.Rotation = 90
	UIGradient_1.Parent = ShopBT
	
	local Notification_1 = Instance.new("Frame")
	Notification_1.Name = "Notification"
	Notification_1.Visible = false
	Notification_1.AnchorPoint = Vector2.new(1.00, 0.00)
	Notification_1.Size = UDim2.new(0.25, 0.00, 0.25, 0.00)
	Notification_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Notification_1.Position = UDim2.new(1.10, 0.00, -0.05, 0.00)
	Notification_1.BorderSizePixel = 0
	Notification_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	Notification_1.Parent = ShopBT
	
	local UIAspectRatioConstraint_1 = Instance.new("UIAspectRatioConstraint")
	UIAspectRatioConstraint_1.Parent = Notification_1
	
	local UICorner_1 = Instance.new("UICorner")
	UICorner_1.CornerRadius = UDim.new(0.50, 0.00)
	UICorner_1.Parent = Notification_1
	
	local Title_1 = Instance.new("TextLabel")
	Title_1.Name = "Title"
	Title_1.TextWrapped = true
	Title_1.BorderSizePixel = 0
	Title_1.TextScaled = true
	Title_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	Title_1.FontFace = Font.new("rbxasset://fonts/families/FredokaOne.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
	Title_1.AnchorPoint = Vector2.new(0.50, 0.50)
	Title_1.TextSize = 14
	Title_1.Size = UDim2.new(0.85, 0.00, 0.90, 0.00)
	Title_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Title_1.Text = "!"
	Title_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
	Title_1.BackgroundTransparency = 1
	Title_1.Position = UDim2.new(0.50, 0.00, 0.50, 0.00)
	Title_1.Parent = Notification_1
	
	local UIStroke_1 = Instance.new("UIStroke")
	UIStroke_1.Color = Color3.new(0.37, 0.00, 0.00)
	UIStroke_1.Thickness = 2
	UIStroke_1.Transparency = 0.30000001192092896
	UIStroke_1.Parent = Notification_1
	
	local UIStroke_1 = Instance.new("UIStroke")
	UIStroke_1.Color = Color3.new(1.00, 1.00, 1.00)
	UIStroke_1.Thickness = 1.7999999523162842
	UIStroke_1.Transparency = 0.6499999761581421
	UIStroke_1.Parent = Notification_1
	
	local UIGradient_1 = Instance.new("UIGradient")
	UIGradient_1.Color = ColorSequence.new(ColorSequenceKeypoint.new(0.00, Color3.new(0.55, 0.21, 0.21)), ColorSequenceKeypoint.new(1.00, Color3.new(1.00, 0.22, 0.22)))
	UIGradient_1.Rotation = 90
	UIGradient_1.Parent = Notification_1
	
	local Button_1 = Instance.new("TextButton")
	Button_1.Name = "Button"
	Button_1.BorderSizePixel = 0
	Button_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	Button_1.FontFace = Font.new("rbxasset://fonts/families/SourceSansPro.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
	Button_1.AnchorPoint = Vector2.new(0.50, 0.50)
	Button_1.TextSize = 14
	Button_1.Size = UDim2.new(1.00, 0.00, 1.00, 0.00)
	Button_1.TextColor3 = Color3.new(0.00, 0.00, 0.00)
	Button_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Button_1.Text = ""
	Button_1.BackgroundTransparency = 1
	Button_1.Position = UDim2.new(0.50, 0.00, 0.50, 0.00)
	Button_1.Parent = ShopBT
	
			STARTER PLAYER:
				local StarterPlayer = game:GetService("StarterPlayer")

			local Client = Instance.new("LocalScript")
			Client.Name = "Client"
			Client.Source = "--// Services\nlocal MarketPlaceService = game:GetService(\'MarketplaceService\')\nlocal ReplicatedStorage = game:GetService(\'ReplicatedStorage\')\nlocal SoundService = game:GetService(\'SoundService\')\nlocal Players = game:GetService(\'Players\')\n\n--// Imports\nlocal Short = require(ReplicatedStorage.Short)\nlocal Stat = require(ReplicatedStorage.Stat)\n\n--// Variables\nlocal Player = Players.LocalPlayer\n\nStat.WaitForLoad() -- Wait's until stats are loaded\n\nlocal Remotes = ReplicatedStorage.RemoteEvents\n\nlocal Interface = Player.PlayerGui:WaitForChild(\'Interface\')\nlocal Leftside = Interface.Leftside\nlocal HUD = Interface.HUD\n\nrepeat task.wait() until #ReplicatedStorage.TemplatePlot.Buttons:GetChildren() > 0\nlocal AmountOfButtons = #ReplicatedStorage.TemplatePlot.Buttons:GetChildren()\n\n--// Stats\nlocal Rebirth = Stat.Get(\'Rebirth\')\nlocal Money = Stat.Get(\'Money\')\n\n--// Main\n--------- Sound ---------\nlocal function PlaySound(Sound: Sound)\n	task.spawn(function()\n		local NewSound = Sound:Clone()\n		NewSound.Parent = game:GetService(\'SoundService\')\n		NewSound:Play()\n		task.wait(5)\n		NewSound:Destroy()\n	end)\nend\n\n--------- Particle ----------\nlocal function SetupButtons()\n	for i = 1, AmountOfButtons do\n		local Stat = Stat.Get(\'Button\'..i)\n\n		Stat.Changed:Connect(function()\n			if not Stat.Value then return end\n\n			local Confetti = script.Confetti:Clone()\n			Confetti.Position = Player.Character.HumanoidRootPart.Position\n			Confetti.Parent = workspace\n\n			Confetti.Attachment.Particle:Emit(45)\n			PlaySound(script.Reward)\n\n			task.wait(3)\n			Confetti:Destroy()		\n		end)\n	end\nend\n\n--------- User Interface ---------\nlocal function CreateSideButtons()\n	Leftside.RebirthBT.Button.MouseButton1Click:Connect(function()\n		HUD.Rebirth.Visible = not HUD.Rebirth.Visible\n	end)\n\n	Leftside.ShopBT.Button.MouseButton1Click:Connect(function()\n		HUD.Shop.Visible = not HUD.Shop.Visible\n	end)\nend\n\nlocal function CreateCloseButtons()\n	HUD.Rebirth.Close.Button.MouseButton1Click:Connect(function()\n		HUD.Rebirth.Visible = false\n	end)\n\n	HUD.Shop.Close.Button.MouseButton1Click:Connect(function()\n		HUD.Shop.Visible = false\n	end)\nend\n\n--------- Currency Label ---------\nlocal function OnMoneyChanged()\n	HUD.MoneyLabel.Main.Text = \'$\'..Short.toSuffix(Money.Value)\nend\n\n--// Rebirth Frame\nlocal function OnRebirthBuy()\n	HUD.Rebirth.Visible = false\n	Remotes.BuyRebirth:FireServer()\nend\n\nlocal PriceStr = 'To Rebirth you need <font color=\'rgb(15, 208, 12)\'>%s </font>💸'\nlocal MultiStr = 'Current Multiplier:  <font color=\'rgb(15, 208, 12)\'>x%s </font>💸'\n\nlocal RebirthPrice = ReplicatedStorage[\'Game Settings\'].Balancing.RebirthPrice.Value\n\nlocal function UpdateRebirthUI()\n	local RebirthVal = Stat.Get(\'Rebirth\').Value\n\n	local Price = Short.toSuffix(RebirthPrice * (RebirthVal + 1))\n	HUD.Rebirth.Price.Text = string.format(PriceStr, Price)\n\n	local Multi = 1 + RebirthVal * 0.5 -- 1 + 0.5x per rebirth\n	HUD.Rebirth.Multi.Text = string.format(MultiStr, Multi)\nend\n\n--// Shop Frame\n-- Credits to Panko_Danko for creating this!\n\nlocal Template = HUD.Shop.ObjectHolder.GamepassFrame\nTemplate.Visible = false\n\nfor _, GamepassInstance in ReplicatedStorage.GamepassIds:GetChildren() do \n	local Id = GamepassInstance.Value\n	local Info = MarketPlaceService:GetProductInfo(Id, Enum.InfoType.GamePass)\n\n	local Frame = Template:Clone()\n	Frame.Title.Text = Info.Name\n	Frame.Description.Text = Info.Description\n	Frame.Price.Text = Info.PriceInRobux .. \' Robux\'\n	Frame.Icon.Image = \'rbxassetid://\'..Info.IconImageAssetId\n\n	if not MarketPlaceService:UserOwnsGamePassAsync(Player.UserId, Id) then\n		Frame.BuyButton.MouseButton1Click:Connect(function()\n			MarketPlaceService:PromptGamePassPurchase(Player, Id)\n		end)\n	else\n		Frame.BuyButton.Text = \'Bought\'\n		Frame.BuyButton.BackgroundColor3 = Color3.fromRGB(7, 136, 0)\n		Frame.BuyButton.UIStroke1.Color = Color3.fromRGB(0, 0, 0)\n		Frame.BuyButton.UIStroke2.Color = Color3.fromRGB(0, 0, 0)\n	end\n\n	Frame.Visible = true\n	Frame.Parent = HUD.Shop.ObjectHolder\nend\n\n--// Connections\nMoney.Changed:Connect(OnMoneyChanged)\nHUD.Rebirth.Buy.Button.MouseButton1Click:Connect(OnRebirthBuy)\nRebirth.Changed:Connect(UpdateRebirthUI)\n\n--// Calls\nOnMoneyChanged()\nUpdateRebirthUI()\nSetupButtons() -- Workspace\nCreateSideButtons() -- UI\nCreateCloseButtons() -- UI"
			Client.Parent = StarterPlayerScripts

			local Confetti = Instance.new("Part")
			Confetti.Name = "Confetti"
			Confetti.TopSurface = Enum.SurfaceType.Smooth
			Confetti.Anchored = true
			Confetti.Size = Vector3.new(1.00, 1.00, 1.00)
			Confetti.BottomSurface = Enum.SurfaceType.Smooth
			Confetti.CanCollide = false
			Confetti.Transparency = 1
			Confetti.BrickColor = BrickColor.new("Medium stone grey")
			Confetti.Position = Vector3.new(12.00, 1.00, -17.00)
			Confetti.CFrame = CFrame.new(12.00, 1.00, -17.00, -0.00, -0.00, -1.00)
			Confetti.Parent = Client

			local Attachment = Instance.new("Attachment")
			Attachment.WorldCFrame = CFrame.new(12.00, 1.00, -17.00, -0.00, -0.00, -1.00)
			Attachment.WorldPosition = Vector3.new(12.00, 1.00, -17.00)
			Attachment.Parent = Confetti

			local Particle = Instance.new("ParticleEmitter")
			Particle.Name = "Particle"
			Particle.Lifetime = NumberRange.new(0.60, 1.50)
			Particle.Color = ColorSequence.new(ColorSequenceKeypoint.new(0.00, Color3.new(1.00, 1.00, 0.00)), ColorSequenceKeypoint.new(1.00, Color3.new(1.00, 0.13, 0.15)))
			Particle.Drag = 7
			Particle.ZOffset = 1.899999976158142
			Particle.LightEmission = 1
			Particle.SpreadAngle = Vector2.new(360.00, -360.00)
			Particle.Speed = NumberRange.new(30.00, 50.00)
			Particle.Brightness = 5
			Particle.Texture = "rbxassetid://11932690139"
			Particle.Enabled = false
			Particle.Acceleration = Vector3.new(0.00, 12.00, 0.00)
			Particle.RotSpeed = NumberRange.new(-360.00, 360.00)
			Particle.Rotation = NumberRange.new(-360.00, 360.00)
			Particle.Rate = 100
			Particle.Size = NumberSequence.new(NumberSequenceKeypoint.new(0.00, 0.00, 0.00), NumberSequenceKeypoint.new(0.10, 1.06, 0.10), NumberSequenceKeypoint.new(0.42, 0.37, 0.00), NumberSequenceKeypoint.new(0.70, 1.06, 0.09), NumberSequenceKeypoint.new(1.00, 0.00, 0.00))
			Particle.Parent = Attachment

			local Reward = Instance.new("Sound")
			Reward.Name = "Reward"
			Reward.SoundId = "rbxassetid://1210852193"
			Reward.Parent = Client
