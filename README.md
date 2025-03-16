

-- Made by GalazySide, Edited by LucaDaBoy

local Upgrader = script.Parent
local Multiplier = Upgrader.Multiplier.Value

local PartsUpgraded = {}

local function onTouched(hit)
	if not hit:IsDescendantOf(workspace.DropperParts) then return end
	if PartsUpgraded[hit] then return end
	
	hit.Worth.Value *= Multiplier
	
	-- So it's only upgraded once, one collision
	PartsUpgraded[hit] = true
	task.wait(10)
	PartsUpgraded[hit] = nil
end

-- Connect the Touched event to the function
Upgrader.Touched:Connect(onTouched)



local Multipliers = Instance.new("ModuleScript")
Multipliers.Name = "Multipliers"
Multipliers.Source = "-- In this module you can edit the multiplier's in game.\n\nlocal Multipliers = {}\n\n--// Services\nlocal ReplicatedStorage = game:GetService(\'ReplicatedStorage\')\n\n--// Imports\nlocal Stat = require(ReplicatedStorage.Stat)\n\n--// Main\nfunction Multipliers.GetMoneyMultiplier(Player)\n	local Multi = 1\n	\n	-- Gamepass\n	local DoubleMoneyExists = ReplicatedStorage.GamepassIds:FindFirstChild(\'DoubleMoney\')\n	\n	if DoubleMoneyExists then\n		local DoubleMoneyOwned = Stat.Get(Player, \'DoubleMoney\').Value\n		\n		if DoubleMoneyOwned then\n			Multi *= 2\n		end\n	end\n	\n	-- Rebirth\n	local Rebirth = Stat.Get(Player, \'Rebirth\')\n	Multi *= (Rebirth.Value + 1)\n	\n	return Multi	\nend\n\nreturn Multipliers"
Multipliers.Parent = game:GetService("ReplicatedStorage")










local Short = Instance.new("ModuleScript")
Short.Name = "Short"
Short.Source = "-- i will one day optimize this module\n\nlocal Module = {}\n\nModule.Prefixes = {\'K\',\'M\',\'B\',\'T\',\'Qd\',\'Qn\',\'Sx\',\'Sp\',\'Oc\',\'No\',\n	\'De\',\'UDe\',\'DDe\',\'TDe\',\'QtDe\',\'QnDe\',\'SxDe\',\'SpDe\',\'OcDe\',\'NoDe\',\n	\'Vg\',\'UVg\',\'DVg\',\'TVg\',\'QdVg\',\'QnVg\',\'SxVg\',\'SpVg\',\'OcVg\',\'NoVg\',\n	\'Tg\',\'UTg\',\'DTg\',\'TTg\',\'QdTg\',\'QnTg\',\'SxTg\',\'SpTg\',\'OcTg\',\'NoTg\',\n	\'qg\',\'Uqg\',\'Dqg\',\'Tqg\',\'Qdqg\',\'Qnqg\',\'Sxqg\',\'Spqg\',\'Ocqg\',\'Noqg\',\n	\'Qg\',\'UQg\',\'DQg\',\'TQg\',\'QdQg\',\'QnQg\',\'SxQg\',\'SpQg\',\'OcQg\',\'NoQg\',\n	\'sg\',\'Usg\',\'Dsg\',\'Tsg\',\'Qdsg\',\'Qnsg\',\'Sxsg\',\'Spsg\',\'Ocsg\',\'Nosg\',\n	\'Sg\',\'USg\',\'DSg\',\'TSg\',\'QdSg\',\'QnSg\',\'SxSg\',\'SpSg\',\'OcSg\',\'NoSg\',\n	\'Og\',\'UOg\',\'DOg\',\'TOg\',\'QdOg\',\'QnOg\',\'SxOg\',\'SpOg\',\'OcOg\',\'NoOg\',\n	\'Ng\',\'UNg\',\'DNg\',\'TNg\',\'QdNg\',\'QnNg\',\'SxNg\',\'SpNg\',\'OcNg\',\'NoNg\',\n	\'Ce\'}\n\n\nfunction Module.CutDigits(x)\n	if x - math.floor(x) == 0 then return x end\n	return string.format(\'%.2f\', x)\nend\n\n\nfunction Module.toSuffix(number, digits)\n	if number == 0 then return number end\n	if number < 1 then return Module.CutDigits(number) end\n	\n	number = (number < 0 and math.abs(number)) or number\n	digits = digits or 2\n	\n	local suffix = math.floor(math.log10(number)/3)\n	\n	return Module.CutDigits(number / 1000^(suffix)) .. ( Module.Prefixes[math.floor(suffix)] or \'\')\nend\n\nfunction Module.toTime(val)\n	if not tonumber(val) then return val end\n\n	local days = math.floor(val / 86400)\n	val = val - days * 86400\n\n	local hours = math.floor(val / 3600)\n	val = val - hours * 3600\n\n	local mins = math.floor(val / 60)\n	val = val - mins * 60\n\n	val = val > 0 and \' \' .. math.floor(val) .. \'s\' or \'\'\n	return (days > 0 and days .. \'d\' or \'\') .. (hours > 0 and \' \' .. hours .. \'h\' or \'\') .. (mins > 0 and \' \' .. mins .. \'m\' or \'\') .. val\nend\n\nfunction Module.toDate(val)\n	if not tonumber(val) then return val end\n	\n	local DateTable = os.date(\'!*t\', val)\n	local Months = {\'Jan\',\'Feb\',\'Mar\',\'Apr\',\'May\',\'Jun\',\'Jul\',\'Aug\',\'Sep\',\'Oct\',\'Nov\',\'Dec\'}\n	\n	return DateTable.day..\' \'..Months[DateTable.month]..\' \'..DateTable.year\nend\n\nreturn Module"
Short.Parent = game:GetService("ReplicatedStorage")










local Stat = Instance.new("ModuleScript")
Stat.Name = "Stat"
Stat.Source = "--[[\nHOW TO USE THIS MODULE\n\nStat.Get(Player, StatName(string)) returns the Stat instance, looks through all folders in ReplicatedStorage.Data until it's found.\nStat.GetDataFolder(Player) returns ReplicatedStorage.Data[PlayerName]\nStat.WaitForLoad(Player) loads and returns a boolean wether the loading succeeded or not.\n\n]]\n\nlocal Stat = {}\nStat.Cached = {} -- Stat's that have been looked up previously are stored here. This makes it so there's no searching the 2nd time you use it\n\nlocal Data\n\nlocal function CreatePath(EndInstance, StartInstance)\n	local Path = {}\n	local CurrentLayer = StartInstance\n	repeat -- loop that imports the names of the parents\n		table.insert(Path, 1, CurrentLayer.Parent.Name)\n		CurrentLayer = CurrentLayer.Parent\n	until -- until the parent is the playerdata\n	CurrentLayer.Parent == EndInstance\n	return Path\nend\n\nlocal function ReadPath(Path, StartInstance)\n	local StatInstance = StartInstance\n	for _, Child in Path do\n		StatInstance = StatInstance[Child] -- this creates the path one by one\n	end\n	return StatInstance\nend\n\nfunction Stat.Get(Player: Player, StatName: string) -- returns stat instance\n	if StatName == nil then -- the Player argument is actually the StatName, and StatName is nil, aka its called from the client\n		StatName = Player\n		Player = game.Players.LocalPlayer\n	end\n	\n	if not Data then\n		Data = game.ReplicatedStorage:WaitForChild(\'Data\')\n	end\n\n	local PlayerData = Data:FindFirstChild(Player.Name)\n	\n	if not PlayerData then\n		task.wait(0.1)\n		return Stat.Get(Player, StatName)\n	end\n\n	local CachedStat = Stat.Cached[StatName]\n	if CachedStat then -- stat is being looked up for the second time if this is true\n		return CachedStat == {} and PlayerData[StatName] or ReadPath(CachedStat, PlayerData)[StatName] -- returns a StatInstance\n	end\n\n	-- first time u look up the stat\n	if PlayerData.Stats:FindFirstChild(StatName) then\n		Stat.Cached[StatName] = {\'Stats\'}\n		return PlayerData.Stats[StatName]\n	else\n		for _,v in PlayerData:GetDescendants() do\n			if v.Name == StatName then\n				Stat.Cached[StatName] = {}\n\n				--// Creates a path and puts it into the Cached folder so it can be accessed directly next time the stat is looked up\n				if v.Parent ~= PlayerData then -- check if it even has a path\n					Stat.Cached[StatName] = CreatePath(PlayerData, v) -- creates a table with the childnames to create the path\n				end\n\n				return v\n			end\n		end\n	end\n	\n	return nil\nend\n\nfunction Stat.GetDataFolder(Player: Player)\n	if not Data then\n		Data = game.ReplicatedStorage.Data\n	end\n	\n	return Data[Player.Name]\nend\n\nfunction Stat.WaitForLoad(Player: any): boolean\n	Player = Player or game.Players.LocalPlayer	\n	repeat wait() until Player:FindFirstChild(\'Loaded\') and Player.Loaded.Value and Player.Parent ~= nil\n	\n	return Player.Parent ~= nil\nend\n\nreturn Stat"
Stat.Parent = game:GetService("ReplicatedStorage")








local Datastore = Instance.new("Folder")
Datastore.Name = "Datastore"
Datastore.Parent = game:GetService("ServerScriptService")

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


local PlotHandler = Instance.new("Script")
PlotHandler.Name = "PlotHandler"
PlotHandler.Source = "--// Services\nlocal MarketPlaceService = game:GetService(\'MarketplaceService\')\nlocal ReplicatedStorage = game:GetService(\'ReplicatedStorage\')\nlocal Players = game:GetService(\'Players\')\n\n--// Requires\nlocal Multipliers = require(ReplicatedStorage.Multipliers)\nlocal Stat = require(ReplicatedStorage.Stat)\n\n--// Variables\nlocal Plots = workspace.Plots\nlocal DropperParts\n\nlocal TemplatePlot = ReplicatedStorage.TemplatePlot\n\nlocal GameType = ReplicatedStorage[\'Game Settings\'].GameType.Value\n\n--// Functions\nlocal function MoveButton(Button, Plot)\n	local RelativeCFrame = TemplatePlot.Ground.CFrame:ToObjectSpace(Button.CFrame)\n	Button.CFrame = Plot.Ground.CFrame:ToWorldSpace(RelativeCFrame)\nend\n\nlocal function HideButton(Button) -- Edit this if you have a different button model!\n	Button.Transparency = 1\n	Button.CanCollide = false\n	Button.BillboardGui.Enabled = false\n	Button.CanTouch = false\nend\n\nlocal function ShowButton(Button) -- Edit this if you have a different button model!\n	Button.Transparency = 0\n	Button.CanCollide = true\n	Button.BillboardGui.Enabled = true\n	Button.CanTouch = true\nend\n\nlocal function MoveUpgrade(Upgrade, Plot)\n	local RelativeCFrame = TemplatePlot.Ground.CFrame:ToObjectSpace(Upgrade:GetPivot())\n	Upgrade:PivotTo(Plot.Ground.CFrame:ToWorldSpace(RelativeCFrame))\nend\n\nlocal function LoadPlot(Player, Plot)\n	if not Plots:FindFirstChild(Plot) then return end\n\n	for i = 1, #TemplatePlot.Buttons:GetChildren() do\n		local Button = Stat.Get(Player, \'Button\'..i)\n\n		if not Button.Value then\n			local NewButton = TemplatePlot.Buttons[i]:Clone()\n			MoveButton(NewButton, Plots[Plot])\n			NewButton.BillboardGui.Price.Text = \'$\'..NewButton.Price.Value\n			NewButton.Parent = Plots[Plot].Buttons\n\n			if ReplicatedStorage[\'Game Settings\'].GameType.Value == \'Modern\' then \n				NewButton.BillboardGui.Income.Text = `+{NewButton.Income.Value}$ /s` 	\n			end\n\n			if NewButton.UnlockedByButton.Value ~= 0 then -- Button isn't unlocked from the start	\n				local CanSee = Stat.Get(Player, \'Button\'..NewButton.UnlockedByButton.Value)\n\n				if not CanSee.Value then -- If the player can not see this then hide the button\n					HideButton(NewButton)\n\n					--// This code waits until you unlocked the necessary button and then makes this one visible again\n					local Connection\n					Connection = CanSee.Changed:Connect(function()\n						ShowButton(NewButton)\n						Connection:Disconnect()\n					end)\n				end\n			end\n\n			local Touched = false\n			NewButton.Touched:Connect(function(Hit)\n				if Touched then return end\n				if not Hit.Parent:FindFirstChild(\'Humanoid\') then return end\n				if Players:GetPlayerFromCharacter(Hit.Parent) == Player then\n					local Currency = Stat.Get(Player, \'Money\')\n					if Currency.Value < NewButton.Price.Value then return end -- Can't afford it!\n					Touched = true\n\n					--// Make the data change\n					Currency.Value -= NewButton.Price.Value\n					Button.Value = true\n\n					--// Make the actual tycoon change\n					local NewUpgrade = TemplatePlot.Upgrades[i]:Clone()\n					MoveUpgrade(NewUpgrade, Plots[Plot])\n					NewUpgrade.Parent = Plots[Plot].Upgrades		\n					NewButton:Destroy()\n\n					if NewUpgrade:FindFirstChild(\'Conveyor\') then\n						NewUpgrade.Conveyor.ConveyorScript.Enabled = true\n					elseif NewUpgrade:FindFirstChild(\'Killpart\') then\n						NewUpgrade.KillHandler.Enabled = true\n					end\n				end\n			end)\n		else\n			local NewUpgrade = TemplatePlot.Upgrades[i]:Clone()\n			MoveUpgrade(NewUpgrade, Plots[Plot])\n			NewUpgrade.Parent = Plots[Plot].Upgrades\n\n			if NewUpgrade:FindFirstChild(\'Conveyor\') then\n				NewUpgrade.Conveyor.ConveyorScript.Enabled = true\n			elseif NewUpgrade:FindFirstChild(\'Killpart\') then\n				NewUpgrade.KillHandler.Enabled = true\n			end\n		end\n	end\n\n	for i = 1, #TemplatePlot.RobuxButtons:GetChildren() do\n		local NewButton = TemplatePlot.RobuxButtons[i]:Clone()\n		MoveButton(NewButton, Plots[Plot])\n\n		local Info = MarketPlaceService:GetProductInfo(NewButton.ProductId.Value, Enum.InfoType.Product)\n		NewButton.BillboardGui.Price.Text = Info.PriceInRobux.. \' Robux\'		\n		NewButton.Parent = Plots[Plot].RobuxButtons\n\n		NewButton.Touched:Connect(function(Hit)\n			if Hit.Parent:FindFirstChild(\'Humanoid\') and Players:GetPlayerFromCharacter(Hit.Parent) == Player then\n				MarketPlaceService:PromptProductPurchase(Player, NewButton.ProductId.Value)\n			end\n		end)\n	end\nend\n\nlocal function ClearPlot(Plot)\n	Plot = Plots[Plot]\n\n	for _, Button in Plot.Buttons:GetChildren() do\n		Button:Destroy()\n	end\n\n	for _, RobuxButton in Plot.RobuxButtons:GetChildren() do\n		RobuxButton:Destroy()\n	end\n\n	for _, Upgrade in Plot.Upgrades:GetChildren() do\n		Upgrade:Destroy()\n	end\nend \n\n--// Player stuff ig\nlocal function OnPlayerRemoving(Player)\n	local Plot = Player.TempValues.Plot.Value\n	if Plot == 0 then return end -- Player has no plot\n\n	local PlotInstance = Plots[Plot]\n	PlotInstance.Claimed.Value = \'None\'\n	PlotInstance.Door.Claim.SurfaceGui.TextLabel.Text = \'Claim\'\n\n	ClearPlot(Plot)\n	Player.TempValues.Plot.Value = 0\n\n	-- Remove player's DropperParts folder\n	local PlayerDropperPartsFolder = workspace.DropperParts:FindFirstChild(Player.Name .. \'-DropperParts\')\n	if PlayerDropperPartsFolder then\n		PlayerDropperPartsFolder:Destroy()\n	end\nend\n\nlocal function OnPlayerAdded(Player)\n	if not Stat.WaitForLoad(Player) then return end -- player left!\n\n	local Plot = Player.TempValues.Plot\n\n	Plot.Changed:Connect(function()\n		LoadPlot(Player, Plot.Value)\n	end)\n\n	Stat.Get(Player, \'Rebirth\').Changed:Connect(function()\n		ClearPlot(Plot.Value)\n		LoadPlot(Player, Plot.Value)\n	end)\n\n	-- Create Button Values\n	for i = 1, #TemplatePlot.Buttons:GetChildren() do\n		if not Stat.Get(Player, \'Button\'..i) then\n			local NewButton = Instance.new(\'BoolValue\')\n			NewButton.Name = \'Button\'..i\n			NewButton.Parent = Stat.GetDataFolder(Player).Buttons\n		end\n	end\n\n	if GameType == \'Classic\' then\n		-- Create DropperParts folder for player\n		local PlayerDropperPartsFolder = Instance.new(\'Folder\')\n		PlayerDropperPartsFolder.Name = Player.Name .. \'-DropperParts\'\n		PlayerDropperPartsFolder.Parent = DropperParts\n	elseif GameType == \'Modern\' then\n		-- For modern tycoons, different income system\n\n		local TemplateButtons = ReplicatedStorage.TemplatePlot.Buttons:GetChildren()\n\n		while task.wait(1) do\n			if Player.Parent == nil then break end\n			if Player.TempValues.Plot.Value == 0 then continue end -- Player hasn't claimed a tycoon\n\n			local Income = 0\n\n			for _, Button in TemplateButtons do\n				if not Stat.Get(Player, \'Button\'..Button.Name).Value then continue end -- Player doesn't own this\n\n				Income += Button.Income.Value\n			end\n\n			local Currency = Stat.Get(Player, \'Money\')\n			local Rebirth = Stat.Get(Player, \'Rebirth\')\n			Currency.Value += Income * Multipliers.GetMoneyMultiplier(Player)\n		end\n	end\nend\n\n--// Doors\nlocal function CreateDoor(v, Hit)\n	if v.Claimed.Value ~= \'None\' then return end -- Already Claimed\n\n	if Hit.Parent:FindFirstChild(\'Humanoid\') then -- Check if it is a player\n		local Player = Players:GetPlayerFromCharacter(Hit.Parent)\n\n		if Player.TempValues.Plot.Value ~= 0 then return end -- Player already claimed a plot\n\n		--// Update tycoon so it become's the player's\n		Player.TempValues.Plot.Value = tonumber(v.Name)\n		v.Claimed.Value = Player.Name\n		v.Door.Claim.SurfaceGui.TextLabel.Text = Player.Name..\''s Plot\'\n	end\nend\n\nlocal function CreateDoors()\n	for _,v in Plots:GetChildren() do\n		v.Door.Claim.Touched:Connect(function(Hit)\n			CreateDoor(v, Hit)\n		end)\n	end\nend\n\n--// Dropper Parts Folder\nlocal function CreateDropperPartsFolder()\n	if GameType == \'Classic\' then\n		DropperParts = Instance.new(\'Folder\')\n		DropperParts.Name = \'DropperParts\'\n		DropperParts.Parent = workspace\n	end\nend\n\n--// Calls\nCreateDoors()\nCreateDropperPartsFolder()\n\n--// Connections\nPlayers.PlayerAdded:Connect(OnPlayerAdded)\nPlayers.PlayerRemoving:Connect(OnPlayerRemoving)"
PlotHandler.Parent = game:GetService("ServerScriptService")


local RemoteHandler = Instance.new("Script")
RemoteHandler.Name = "RemoteHandler"
RemoteHandler.Source = "--// Services\nlocal ReplicatedStorage = game:GetService(\'ReplicatedStorage\')\n\n--// Requires\nlocal Stat = require(ReplicatedStorage.Stat)\n\n--// Variables\nlocal Remotes = ReplicatedStorage.RemoteEvents\n\nRemotes.BuyRebirth.OnServerEvent:Connect(function(Player) -- Needs a debounce\n	local Money = Stat.Get(Player, \'Money\')\n	local Rebirth = Stat.Get(Player, \'Rebirth\')\n	\n	local RebirthPrice = ReplicatedStorage[\'Game Settings\'].Balancing.RebirthPrice.Value\n	\n	if Money.Value >= RebirthPrice * (Rebirth.Value + 1) then\n		Money.Value = 0\n		\n		local AmountOfButtons = #ReplicatedStorage.TemplatePlot.Buttons:GetChildren()\n		for i = 1, AmountOfButtons do\n			Stat.Get(Player, \'Button\'..i).Value = false	\n		end\n		\n		Rebirth.Value += 1\n		\n		-- Clear Drops\n		local PlayerDropperPartsFolder = workspace.DropperParts:FindFirstChild(Player.Name .. \'-DropperParts\')\n		\n		for _, Drop in PlayerDropperPartsFolder:GetChildren() do\n			Drop:Destroy()\n		end\n	end\nend)"
RemoteHandler.Parent = game:GetService("ServerScriptService")



local RobuxHandler = Instance.new("Script")
RobuxHandler.Name = "RobuxHandler"
RobuxHandler.Source = "--// Services\nlocal MarketPlaceService = game:GetService(\'MarketplaceService\')\nlocal ReplicatedStorage = game:GetService(\'ReplicatedStorage\')\nlocal Players = game:GetService(\'Players\')\n\n--// Imports\nlocal Stat = require(ReplicatedStorage.Stat)\n\n--// Variables\nlocal GamepassIds = ReplicatedStorage.GamepassIds\n\n--// Functions\nlocal function AwardTool(Player, ToolName)\n	local Tool = script:FindFirstChild(ToolName):Clone()\n\n	if not Tool then\n		warn(\'Error awarding gamepass reward, \'..ToolName..\' does not exist!\')\n		return -- An error occured, stop the function from running\n	end\n\n	Tool:Clone().Parent = Player.Backpack	\nend\n\nlocal function CreateGamepasses(Player)\n	local Data = Stat.GetDataFolder(Player)\n	for _, GamepassInstance in GamepassIds:GetChildren() do\n		local GPVal = Data.Other:FindFirstChild(GamepassInstance.Name)\n\n		-- Create a gamepass if it doesn't exist\n		if not GPVal then\n			GPVal = Instance.new(\'BoolValue\')\n			GPVal.Name = GamepassInstance.Name\n			GPVal.Parent = Data.Other\n		end\n\n		if MarketPlaceService:UserOwnsGamePassAsync(Player.UserId, GamepassInstance.Value) then\n			GPVal.Value = true\n		end \n	end\nend\n\nlocal function OnCharacterAdded(Character) -- Function loads in the tools\n	local Player = Players:GetPlayerFromCharacter(Character)\n\n	for _, GamepassInstance in GamepassIds:GetChildren() do\n		if not script:FindFirstChild(GamepassInstance.Name) then continue end -- Gamepass has no tool\n\n		if Stat.Get(Player, GamepassInstance.Name).Value == false then continue end\n\n		AwardTool(Player, GamepassInstance.Name)\n	end\nend\n\nfunction OnPlayerAdded(Player)\n	Stat.WaitForLoad(Player)\n	CreateGamepasses(Player) -- Creates the values\n\n	local Character = Player.Character or Player.CharacterAdded:Wait()\n\n	Player.CharacterAdded:Connect(OnCharacterAdded)\n	OnCharacterAdded(Character)\nend\n\nfunction OnGamepassPurchaseFinished(Player, GamepassId, Purchased)\n	if not Purchased then return end\n\n	for _, GamepassInstance in GamepassIds:GetChildren() do\n		if GamepassInstance.Value == GamepassId then\n			AwardTool(Player, GamepassInstance.Name)\n			break\n		end\n	end\nend\n\nfunction ProcessReceipt(ReceiptInfo)\n	local Player = Players:GetPlayerByUserId(ReceiptInfo.PlayerId)\n\n	for _, Button in ReplicatedStorage.TemplatePlot.RobuxButtons:GetChildren() do\n		if Button.ProductId.Value == ReceiptInfo.ProductId then\n			local Amount = Button.Amount.Value\n			local Money = Stat.Get(Player, \'Money\')\n			Money.Value += Amount\n			break\n		end\n	end\n\n	return Enum.ProductPurchaseDecision.PurchaseGranted\nend\n\n--// Main\nPlayers.PlayerAdded:Connect(OnPlayerAdded)\n\nMarketPlaceService.PromptGamePassPurchaseFinished:Connect(OnGamepassPurchaseFinished)\n\nMarketPlaceService.ProcessReceipt = ProcessReceipt"
RobuxHandler.Parent = game:GetService("ServerScriptService")

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
RightGripAttachment_1.Parent = Handle_1


local Script_1 = Instance.new("Script")
Script_1.Source = "-- Scripted by emblazes, rescripted by LucaDaBoy\n\n--// Services\nlocal Players = game:GetService(\'Players\')\n\n--// Variables\nlocal GravityCoil = script.Parent\nlocal Handle = GravityCoil.Handle\n\n\nlocal Sounds = {CoilSound = Handle.CoilSound,}\n\nlocal Gravity = 196.20\nlocal JumpHeightPercentage = 0.25\n\nlocal ToolEquipped = false\n\n--// Functions\nfunction GetAllConnectedParts(Object)\n	local Parts = {}\n	local function GetConnectedParts(Object)\n		for i, v in Object:GetConnectedParts() do\n			local Ignore = false\n			for ii, vv in Parts do\n				if v == vv then\n					Ignore = true\n				end\n			end\n			if not Ignore then\n				table.insert(Parts, v)\n				GetConnectedParts(v)\n			end\n		end\n	end\n	GetConnectedParts(Object)\n	return Parts\nend\n\nfunction SetGravityEffect()\n	if not GravityEffect or not GravityEffect.Parent then\n		GravityEffect = Instance.new(\'BodyForce\')\n		GravityEffect.Name = \'GravityCoilEffect\'\n		GravityEffect.Parent = Torso\n	end\n	\n	local TotalMass = 0\n	local ConnectedParts = GetAllConnectedParts(Torso)\n	\n	for _,v in ConnectedParts do\n		if v:IsA(\'BasePart\') then\n			TotalMass = (TotalMass + v:GetMass())\n		end\n	end\n	\n	local TotalMass = (TotalMass * 196.20 * (1 - JumpHeightPercentage))\n	GravityEffect.force = Vector3.new(0, TotalMass, 0)\nend\n\nfunction HandleGravityEffect(Enabled)\n	if not CheckIfAlive() then return end\n	\n	for _,v in Torso:GetChildren() do\n		if v:IsA(\'BodyForce\') then\n			v:Destroy()\n		end\n	end\n	\n	if not Enabled then return end\n\n	local CurrentlyEquipped = true\n	\n	GravityCoil.Unequipped:connect(function()\n		CurrentlyEquipped = false\n	end)\n	\n	SetGravityEffect()\n	\n	Character.DescendantAdded:connect(function()\n		task.wait()\n		if not CurrentlyEquipped or not CheckIfAlive() then\n			return\n		end\n		SetGravityEffect()\n	end)\n	\n	Character.DescendantRemoving:connect(function()\n		task.wait()\n		if not CurrentlyEquipped or not CheckIfAlive() then\n			return\n		end\n		SetGravityEffect()\n	end)\nend\n\nfunction CheckIfAlive()\n	return (((Character and Character.Parent and Humanoid and Humanoid.Parent and Humanoid.Health > 0 and Torso and Torso.Parent and Player and Player.Parent) and true) or false)\nend\n\nfunction Equipped(Mouse)\n	Character = GravityCoil.Parent\n	Humanoid = Character:FindFirstChild(\'Humanoid\')\n	Torso = Character:FindFirstChild(\'Torso\') or Character:FindFirstChild(\'UpperTorso\')\n	Player = Players:GetPlayerFromCharacter(Character)\n	\n	if not CheckIfAlive() then\n		return\n	end\n	if HumanoidDied then\n		HumanoidDied:Disconnect()\n	end\n	HumanoidDied = Humanoid.Died:connect(function()\n		if GravityEffect and GravityEffect.Parent then\n			GravityEffect:Destroy()\n		end\n	end)\n	Sounds.CoilSound:Play()\n	HandleGravityEffect(true)\n	ToolEquipped = true\nend\n\nfunction Unequipped()\n	if HumanoidDied then\n		HumanoidDied:Disconnect()\n	end\n	HandleGravityEffect(false)\n	ToolEquipped = false\nend\n\n--// Main\nGravityCoil.Equipped:connect(Equipped)\nGravityCoil.Unequipped:connect(Unequipped)"
Script_1.Parent = GravityCoil


local leaderstats = Instance.new("Script")
leaderstats.Name = "leaderstats"
leaderstats.Source = "--// Services\nlocal ReplicatedStorage = game:GetService(\'ReplicatedStorage\')\nlocal Players = game:GetService(\'Players\')\n\nlocal Stat = require(ReplicatedStorage.Stat)\n\nPlayers.PlayerAdded:Connect(function(Player)\n	if not Stat.WaitForLoad(Player) then return end -- player left!\n	\n	local MoneyStat = Stat.Get(Player, \'Money\')\n	\n	local Money = Instance.new(\'NumberValue\', Player.leaderstats)\n	Money.Name = \'Money\'\n	Money.Value = MoneyStat.Value\n	\n	MoneyStat.Changed:Connect(function()\n		Money.Value = MoneyStat.Value\n	end)\nend)"
leaderstats.Parent = game:GetService("ServerScriptService")


local Dropper = Instance.new("ModuleScript")
Dropper.Name = "Dropper"
Dropper.Source = "local Dropper = {}\n\nlocal Stat = require(game.ReplicatedStorage.Stat)\nlocal Multipliers = require(game.ReplicatedStorage.Multipliers)\n\nfunction Dropper.Spawn(Player, Pos, Amount)\n	local NewPart = Instance.new(\'Part\')\n	NewPart.Size = Vector3.new(1,1,1)\n	NewPart.Position = Pos\n	NewPart.Parent = workspace.DropperParts[Player.Name..\'-DropperParts\']\n	\n	local Worth = Instance.new(\'NumberValue\')\n	Worth.Name = \'Worth\'\n	Worth.Value = Amount\n	Worth.Parent = NewPart\n	\n	local Billboard = script.BillboardGui:Clone()\n	Billboard.TextLabel.Text = \'$\'..Worth.Value\n	Billboard.Parent = NewPart\n	\n	Worth.Changed:Connect(function()\n		Billboard.TextLabel.Text = \'$\'..Worth.Value\n	end)\n	\n	task.spawn(function() -- Despawn after 30 seconds\n		task.wait(30)\n		NewPart:Destroy()\n	end)\n	\n	local Currency = Stat.Get(Player, \'Money\')\n	local Rebirth = Stat.Get(Player, \'Rebirth\')\n	\n	NewPart.Touched:Connect(function(Hit)\n		if Hit.Name == \'Furnace\' then\n			Currency.Value += Worth.Value * Multipliers.GetMoneyMultiplier(Player)\n			NewPart:Destroy()\n		elseif Hit.Name == \'Ground\' then\n			NewPart:Destroy()\n		end\n	end)\nend\n\nreturn Dropper"
Dropper.Parent = game:GetService("ServerScriptService")

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






local Client = Instance.new("LocalScript")
Client.Name = "Client"
Client.Source = "--// Services\nlocal MarketPlaceService = game:GetService(\'MarketplaceService\')\nlocal ReplicatedStorage = game:GetService(\'ReplicatedStorage\')\nlocal SoundService = game:GetService(\'SoundService\')\nlocal Players = game:GetService(\'Players\')\n\n--// Imports\nlocal Short = require(ReplicatedStorage.Short)\nlocal Stat = require(ReplicatedStorage.Stat)\n\n--// Variables\nlocal Player = Players.LocalPlayer\n\nStat.WaitForLoad() -- Wait's until stats are loaded\n\nlocal Remotes = ReplicatedStorage.RemoteEvents\n\nlocal Interface = Player.PlayerGui:WaitForChild(\'Interface\')\nlocal Leftside = Interface.Leftside\nlocal HUD = Interface.HUD\n\nrepeat task.wait() until #ReplicatedStorage.TemplatePlot.Buttons:GetChildren() > 0\nlocal AmountOfButtons = #ReplicatedStorage.TemplatePlot.Buttons:GetChildren()\n\n--// Stats\nlocal Rebirth = Stat.Get(\'Rebirth\')\nlocal Money = Stat.Get(\'Money\')\n\n--// Main\n--------- Sound ---------\nlocal function PlaySound(Sound: Sound)\n	task.spawn(function()\n		local NewSound = Sound:Clone()\n		NewSound.Parent = game:GetService(\'SoundService\')\n		NewSound:Play()\n		task.wait(5)\n		NewSound:Destroy()\n	end)\nend\n\n--------- Particle ----------\nlocal function SetupButtons()\n	for i = 1, AmountOfButtons do\n		local Stat = Stat.Get(\'Button\'..i)\n\n		Stat.Changed:Connect(function()\n			if not Stat.Value then return end\n\n			local Confetti = script.Confetti:Clone()\n			Confetti.Position = Player.Character.HumanoidRootPart.Position\n			Confetti.Parent = workspace\n\n			Confetti.Attachment.Particle:Emit(45)\n			PlaySound(script.Reward)\n\n			task.wait(3)\n			Confetti:Destroy()		\n		end)\n	end\nend\n\n--------- User Interface ---------\nlocal function CreateSideButtons()\n	Leftside.RebirthBT.Button.MouseButton1Click:Connect(function()\n		HUD.Rebirth.Visible = not HUD.Rebirth.Visible\n	end)\n\n	Leftside.ShopBT.Button.MouseButton1Click:Connect(function()\n		HUD.Shop.Visible = not HUD.Shop.Visible\n	end)\nend\n\nlocal function CreateCloseButtons()\n	HUD.Rebirth.Close.Button.MouseButton1Click:Connect(function()\n		HUD.Rebirth.Visible = false\n	end)\n\n	HUD.Shop.Close.Button.MouseButton1Click:Connect(function()\n		HUD.Shop.Visible = false\n	end)\nend\n\n--------- Currency Label ---------\nlocal function OnMoneyChanged()\n	HUD.MoneyLabel.Main.Text = \'$\'..Short.toSuffix(Money.Value)\nend\n\n--// Rebirth Frame\nlocal function OnRebirthBuy()\n	HUD.Rebirth.Visible = false\n	Remotes.BuyRebirth:FireServer()\nend\n\nlocal PriceStr = 'To Rebirth you need <font color=\'rgb(15, 208, 12)\'>%s </font>💸'\nlocal MultiStr = 'Current Multiplier:  <font color=\'rgb(15, 208, 12)\'>x%s </font>💸'\n\nlocal RebirthPrice = ReplicatedStorage[\'Game Settings\'].Balancing.RebirthPrice.Value\n\nlocal function UpdateRebirthUI()\n	local RebirthVal = Stat.Get(\'Rebirth\').Value\n\n	local Price = Short.toSuffix(RebirthPrice * (RebirthVal + 1))\n	HUD.Rebirth.Price.Text = string.format(PriceStr, Price)\n\n	local Multi = 1 + RebirthVal * 0.5 -- 1 + 0.5x per rebirth\n	HUD.Rebirth.Multi.Text = string.format(MultiStr, Multi)\nend\n\n--// Shop Frame\n-- Credits to Panko_Danko for creating this!\n\nlocal Template = HUD.Shop.ObjectHolder.GamepassFrame\nTemplate.Visible = false\n\nfor _, GamepassInstance in ReplicatedStorage.GamepassIds:GetChildren() do \n	local Id = GamepassInstance.Value\n	local Info = MarketPlaceService:GetProductInfo(Id, Enum.InfoType.GamePass)\n\n	local Frame = Template:Clone()\n	Frame.Title.Text = Info.Name\n	Frame.Description.Text = Info.Description\n	Frame.Price.Text = Info.PriceInRobux .. \' Robux\'\n	Frame.Icon.Image = \'rbxassetid://\'..Info.IconImageAssetId\n\n	if not MarketPlaceService:UserOwnsGamePassAsync(Player.UserId, Id) then\n		Frame.BuyButton.MouseButton1Click:Connect(function()\n			MarketPlaceService:PromptGamePassPurchase(Player, Id)\n		end)\n	else\n		Frame.BuyButton.Text = \'Bought\'\n		Frame.BuyButton.BackgroundColor3 = Color3.fromRGB(7, 136, 0)\n		Frame.BuyButton.UIStroke1.Color = Color3.fromRGB(0, 0, 0)\n		Frame.BuyButton.UIStroke2.Color = Color3.fromRGB(0, 0, 0)\n	end\n\n	Frame.Visible = true\n	Frame.Parent = HUD.Shop.ObjectHolder\nend\n\n--// Connections\nMoney.Changed:Connect(OnMoneyChanged)\nHUD.Rebirth.Buy.Button.MouseButton1Click:Connect(OnRebirthBuy)\nRebirth.Changed:Connect(UpdateRebirthUI)\n\n--// Calls\nOnMoneyChanged()\nUpdateRebirthUI()\nSetupButtons() -- Workspace\nCreateSideButtons() -- UI\nCreateCloseButtons() -- UI"
Client.Parent = game:GetService("StarterPlayer"):WaitForChild("StarterPlayerScripts")

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

