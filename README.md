local Library = {}

function Library:CreateWindow(title)
	
	local UILib = Instance.new("ScreenGui")
	local library = Instance.new("Frame")
	local UICorner = Instance.new("UICorner")
	local name = Instance.new("TextLabel")
	local min = Instance.new("ImageButton")
	local close = Instance.new("ImageButton")
	local max = Instance.new("ImageButton")
	
	library.Name = "library"
	library.Parent = UILib
	library.BackgroundColor3 = Color3.fromRGB(34, 34, 34)
	library.Position = UDim2.new(0.0650283843, 0, 0.29111439, 0)
	library.Size = UDim2.new(0, 641, 0, 316)

	UICorner.Parent = library

	name.Name = "name"
	name.Parent = library
	name.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	name.BackgroundTransparency = 1.000
	name.Position = UDim2.new(0.0265210588, 0, 0.0251572337, 0)
	name.Size = UDim2.new(0, 200, 0, 50)
	name.Font = Enum.Font.GothamSemibold
	name.Text = title
	name.TextColor3 = Color3.fromRGB(255, 255, 255)
	name.TextSize = 32.000
	name.TextWrapped = true
	
	local Tabs = {}
	
	function Tabs:CreateTabs(title, callback)
		
		callback = callback or function() end
		
		local Tabs = Instance.new("Frame")
		local tab2 = Instance.new("TextButton")
		local UICorner_2 = Instance.new("UICorner")
		local tab3 = Instance.new("TextButton")
		local UICorner_3 = Instance.new("UICorner")
		local tab1 = Instance.new("TextButton")
		local tabstextlabel = Instance.new("TextLabel")
		local UICorner_4 = Instance.new("UICorner")
		
		Tabs.Name = "Tabs"
		Tabs.Parent = library
		Tabs.BackgroundColor3 = Color3.fromRGB(42, 42, 42)
		Tabs.Position = UDim2.new(0.0452418104, 0, 0.18238993, 0)
		Tabs.Size = UDim2.new(0, 129, 0, 226)

		tab2.Name = "tab2"
		tab2.Parent = Tabs
		tab2.BackgroundColor3 = Color3.fromRGB(65, 65, 65)
		tab2.BorderColor3 = Color3.fromRGB(0, 0, 0)
		tab2.Position = UDim2.new(0.206589103, 0, 0.423896313, 0)
		tab2.Size = UDim2.new(0, 74, 0, 50)
		tab2.Font = Enum.Font.SourceSansLight
		tab2.Text = "Decoder"
		tab2.TextColor3 = Color3.fromRGB(255, 255, 255)
		tab2.TextScaled = true
		tab2.TextSize = 14.000
		tab2.TextWrapped = true
		
		tab2.MouseButton1Down:Connect(function()
			pcall(callback)

		end)

		UICorner_2.Parent = tab2

		tab3.Name = "tab3"
		tab3.Parent = Tabs
		tab3.BackgroundColor3 = Color3.fromRGB(70, 70, 70)
		tab3.BorderColor3 = Color3.fromRGB(0, 0, 0)
		tab3.Position = UDim2.new(0.206589103, 0, 0.729258418, 0)
		tab3.Size = UDim2.new(0, 73, 0, 50)
		tab3.Font = Enum.Font.SourceSansLight
		tab3.Text = "Anti Logger"
		tab3.TextColor3 = Color3.fromRGB(255, 255, 255)
		tab3.TextScaled = true
		tab3.TextSize = 14.000
		tab3.TextWrapped = true
		
		tab3.MouseButton1Down:Connect(function()
			pcall(callback)

		end)

		UICorner_3.Parent = tab3

		tab1.Name = "tab1"
		tab1.Parent = Tabs
		tab1.BackgroundColor3 = Color3.fromRGB(65, 65, 65)
		tab1.BorderColor3 = Color3.fromRGB(0, 0, 0)
		tab1.Position = UDim2.new(0.206589133, 0, 0.115113109, 0)
		tab1.Size = UDim2.new(0, 74, 0, 50)
		tab1.Font = Enum.Font.SourceSansLight
		tab1.Text = "Home"
		tab1.TextColor3 = Color3.fromRGB(255, 255, 255)
		tab1.TextScaled = true
		tab1.TextSize = 24.000
		tab1.TextWrapped = true
		
		tab1.MouseButton1Down:Connect(function()
			pcall(callback)

		end)

		UICorner_4.Parent = tab1

		tabstextlabel.Name = "tabstextlabel"
		tabstextlabel.Parent = Tabs
		tabstextlabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		tabstextlabel.BackgroundTransparency = 1.060
		tabstextlabel.Position = UDim2.new(0.116279073, 0, 0, 0)
		tabstextlabel.Size = UDim2.new(0, 100, 0, 26)
		tabstextlabel.Font = Enum.Font.SourceSansLight
		tabstextlabel.Text = "Tabs :"
		tabstextlabel.TextColor3 = Color3.fromRGB(255, 255, 255)
		tabstextlabel.TextSize = 22.000
		
		
	end
	
	local WelcomeTab = {}
	
	function WelcomeTab:CreateWelTab(title)
		
		local welcome = Instance.new("Frame")
		local playerimg = Instance.new("ImageLabel")
		local UICorner_6 = Instance.new("UICorner")
		local name2 = Instance.new("TextLabel")
		local UICorner_7 = Instance.new("UICorner")
		local devs = Instance.new("TextLabel")
		
		welcome.Name = "welcome"
		welcome.Parent = library
		welcome.BackgroundColor3 = Color3.fromRGB(42, 42, 42)
		welcome.Position = UDim2.new(0.288611531, 0, 0.169811308, 0)
		welcome.Size = UDim2.new(0, 415, 0, 233)

		playerimg.Name = "playerimg"
		playerimg.Parent = welcome
		playerimg.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		playerimg.Position = UDim2.new(0.308008909, 0, 0.060806226, 0)
		playerimg.Size = UDim2.new(0, 128, 0, 120)
		playerimg.Image = "rbxasset://textures/ui/GuiImagePlaceholder.png"

		UICorner_6.CornerRadius = UDim.new(0, 98)
		UICorner_6.Parent = playerimg

		name2.Name = "name2"
		name2.Parent = welcome
		name2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		name2.BackgroundTransparency = 1.000
		name2.Position = UDim2.new(0.239798501, 0, 0.606067896, 0)
		name2.Size = UDim2.new(0, 200, 0, 50)
		name2.Font = Enum.Font.GothamBold
		name2.Text = "Welcome To Skids Hub V3"
		name2.TextColor3 = Color3.fromRGB(255, 255, 255)
		name2.TextSize = 14.000

		UICorner_7.Parent = welcome

		devs.Name = "devs"
		devs.Parent = welcome
		devs.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		devs.BackgroundTransparency = 1.000
		devs.Position = UDim2.new(0.219277114, 0, 0.872162282, 0)
		devs.Size = UDim2.new(0, 200, 0, 29)
		devs.Font = Enum.Font.SourceSansLight
		devs.Text = "Developed by  DARK_MANE#7089 And Emi_H#3854"
		devs.TextColor3 = Color3.fromRGB(255, 255, 255)
		devs.TextSize = 15.000
		
		
	end
	
	local DecoderTab = {}

	function DecoderTab:CreateDecTab(callback)
		
		callback = callback or function() end
		
		local DecoderTab = Instance.new("Frame")
		local UICorner_8 = Instance.new("UICorner")
		local user = Instance.new("TextBox")
		local UICorner_9 = Instance.new("UICorner")
		local decode = Instance.new("TextButton")
		local UICorner_10 = Instance.new("UICorner")
		local decodetext = Instance.new("TextLabel")
		
		DecoderTab.Name = "DecoderTab"
		DecoderTab.Parent = library
		DecoderTab.Active = true
		DecoderTab.BackgroundColor3 = Color3.fromRGB(53, 53, 53)
		DecoderTab.Position = UDim2.new(0.288611531, 0, 0.169811323, 0)
		DecoderTab.Size = UDim2.new(0, 415, 0, 230)
		DecoderTab.Visible = false

		UICorner_8.Parent = DecoderTab

		user.Name = "user"
		user.Parent = DecoderTab
		user.BackgroundColor3 = Color3.fromRGB(45, 45, 45)
		user.Position = UDim2.new(0.240963861, 0, 0.304347813, 0)
		user.Size = UDim2.new(0, 200, 0, 50)
		user.Font = Enum.Font.SourceSansLight
		user.Text = "User Here "
		user.TextColor3 = Color3.fromRGB(255, 255, 255)
		user.TextSize = 23.000

		UICorner_9.Parent = user

		decode.Name = "decode"
		decode.Parent = DecoderTab
		decode.BackgroundColor3 = Color3.fromRGB(45, 45, 45)
		decode.Position = UDim2.new(0.240963861, 0, 0.5826087, 0)
		decode.Size = UDim2.new(0, 200, 0, 50)
		decode.Font = Enum.Font.SourceSansLight
		decode.Text = "Decode"
		decode.TextColor3 = Color3.fromRGB(255, 255, 255)
		decode.TextSize = 37.000
		
		decode.MouseButton1Down:Connect(function()
			pcall(callback)

		end)

		UICorner_10.Parent = decode

		decodetext.Name = "decodetext"
		decodetext.Parent = DecoderTab
		decodetext.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		decodetext.BackgroundTransparency = 0.900
		decodetext.Size = UDim2.new(0, 415, 0, 30)
		decodetext.Font = Enum.Font.SourceSansLight
		decodetext.Text = "Decoder"
		decodetext.TextColor3 = Color3.fromRGB(255, 255, 255)
		decodetext.TextSize = 22.000
		
	end
	
	local AntiTab = {}
	
	function AntiTab:CreateAntiTab(callback)
		
		callback = callback or function() end
		
		local VisualizerTab = Instance.new("Frame")
		local visualize = Instance.new("TextButton")
		local UICorner_13 = Instance.new("UICorner")
		local Sorry2 = Instance.new("ImageLabel")
		local UICorner_14 = Instance.new("UICorner")
		local text123 = Instance.new("TextLabel")
		local play = Instance.new("TextButton")
		local UICorner_15 = Instance.new("UICorner")
		local massplay = Instance.new("TextButton")
		local UICorner_16 = Instance.new("UICorner")
		local Pattern = Instance.new("ImageLabel")
		local UICorner_17 = Instance.new("UICorner")
		
		visualize.Name = "visualize"
		visualize.Parent = VisualizerTab
		visualize.BackgroundColor3 = Color3.fromRGB(40, 40, 40)
		visualize.Position = UDim2.new(0.257831335, 0, 0.653846145, 0)
		visualize.Size = UDim2.new(0, 200, 0, 50)
		visualize.Font = Enum.Font.SourceSansLight
		visualize.Text = "Visualize"
		visualize.TextColor3 = Color3.fromRGB(255, 255, 255)
		visualize.TextSize = 32.000

		UICorner_13.Parent = visualize

		Sorry2.Name = "Sorry2"
		Sorry2.Parent = visualize
		Sorry2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		Sorry2.BackgroundTransparency = 1.000
		Sorry2.Position = UDim2.new(0, 0, 0.0199999996, 0)
		Sorry2.Size = UDim2.new(0, 200, 0, 49)
		Sorry2.ZIndex = 9
		Sorry2.Image = "rbxassetid://300134974"
		Sorry2.ImageTransparency = 0.600
		Sorry2.ScaleType = Enum.ScaleType.Tile
		Sorry2.SliceCenter = Rect.new(0, 256, 0, 256)
		Sorry2.TileSize = UDim2.new(0, 90, 0, 90)

		UICorner_14.Parent = Sorry2

		text123.Name = "text123"
		text123.Parent = VisualizerTab
		text123.Active = true
		text123.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		text123.BackgroundTransparency = 0.950
		text123.Size = UDim2.new(0, 415, 0, 30)
		text123.Font = Enum.Font.SourceSans
		text123.Text = "Visualizer / Mass Play/ Play"
		text123.TextColor3 = Color3.fromRGB(255, 255, 255)
		text123.TextSize = 14.000

		play.Name = "play"
		play.Parent = VisualizerTab
		play.BackgroundColor3 = Color3.fromRGB(42, 42, 42)
		play.Position = UDim2.new(0.0578313246, 0, 0.658119678, 0)
		play.Size = UDim2.new(0, 75, 0, 50)
		play.Font = Enum.Font.SourceSansLight
		play.Text = "Play"
		play.TextColor3 = Color3.fromRGB(255, 255, 255)
		play.TextScaled = true
		play.TextSize = 29.000
		play.TextWrapped = true

		UICorner_15.Parent = play

		massplay.Name = "massplay"
		massplay.Parent = VisualizerTab
		massplay.BackgroundColor3 = Color3.fromRGB(42, 42, 42)
		massplay.Position = UDim2.new(0.766265094, 0, 0.658119678, 0)
		massplay.Size = UDim2.new(0, 82, 0, 50)
		massplay.Font = Enum.Font.SourceSansLight
		massplay.Text = "Massplay"
		massplay.TextColor3 = Color3.fromRGB(255, 255, 255)
		massplay.TextScaled = true
		massplay.TextSize = 14.000
		massplay.TextWrapped = true

		UICorner_16.Parent = massplay

		Pattern.Name = "Pattern"
		Pattern.Parent = massplay
		Pattern.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		Pattern.BackgroundTransparency = 1.000
		Pattern.Size = UDim2.new(0, 82, 0, 51)
		Pattern.ZIndex = 9
		Pattern.Image = "rbxassetid://300134974"
		Pattern.ImageTransparency = 0.600
		Pattern.ScaleType = Enum.ScaleType.Tile
		Pattern.SliceCenter = Rect.new(0, 256, 0, 256)
		Pattern.TileSize = UDim2.new(0, 90, 0, 90)

		UICorner_17.Parent = Pattern
		
		play.MouseButton1Down:Connect(function()
			pcall(callback)

		end)
		
	end
	
	local GetMinMaxClosButtons = {}
	
	function GetMinMaxClosButtons:CreateIt(callback)
		callback = callback or function() end
		
		local min = Instance.new("ImageButton")
		local close = Instance.new("ImageButton")
		local max = Instance.new("ImageButton")
		
		min.Name = "min"
		min.Parent = library
		min.BackgroundTransparency = 1.000
		min.LayoutOrder = 4
		min.Position = UDim2.new(0.856474221, 0, -0.00157725811, 0)
		min.Size = UDim2.new(0, 30, 0, 30)
		min.ZIndex = 2
		min.Image = "rbxassetid://3926307971"
		min.ImageRectOffset = Vector2.new(884, 284)
		min.ImageRectSize = Vector2.new(36, 36)

		close.Name = "close"
		close.Parent = library
		close.BackgroundTransparency = 1.000
		close.Position = UDim2.new(0.952342868, 0, -0.00157725811, 0)
		close.Size = UDim2.new(0, 30, 0, 30)
		close.ZIndex = 2
		close.Image = "rbxassetid://3926305904"
		close.ImageRectOffset = Vector2.new(284, 4)
		close.ImageRectSize = Vector2.new(24, 24)

		max.Name = "max"
		max.Parent = library
		max.BackgroundTransparency = 1.000
		max.LayoutOrder = 11
		max.Position = UDim2.new(0.904056191, 0, -0.00157731771, 0)
		max.Size = UDim2.new(0, 30, 0, 30)
		max.ZIndex = 2
		max.Image = "rbxassetid://3926307971"
		max.ImageRectOffset = Vector2.new(4, 44)
		max.ImageRectSize = Vector2.new(36, 36)
		
		min.MouseButton1Down:Connect(function()
			pcall(callback)
			
		end)
		
		max.MouseButton1Down:Connect(function()
			pcall(callback)

		end)
		
		close.MouseButton1Down:Connect(function()
			pcall(callback)

		end)
		
	end
	
	
end
