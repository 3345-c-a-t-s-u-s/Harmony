# Harmony
```lua
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/3345-c-a-t-s-u-s/Harmony/refs/heads/main/src/init.luau"))();

local Window = Library.new({
	Title = "Harmony Library "..Library.Version,
})

local ExampleTab = Window:AddTab({
	Title = "Example",
	Icon = "book"
});

local SettingsTab = Window:AddTab({
	Title = "Settings",
	Icon = "settings"
});

local GeneralSection = ExampleTab:AddSection({
	Title = "General"
});

local ExampleSection = ExampleTab:AddSection({
	Title = "Automatics"
});

do -- Example
	GeneralSection:AddButton({
		Title = "Button",
		Callback = function()
			print('Click!')
		end,
	});
	
	GeneralSection:AddToggle({
		Title = "Toggle",
		Default = false,
		Callback = function(value)
			print(value)
		end,
	});

	GeneralSection:AddSlider({
		Title = "Slider",
		Min = 1,
		Max = 100,
		Default = 10,
		Rounding = 1,
		Callback = function(value)
			print(value)
		end,
	});
	
	GeneralSection:AddKeybind({
		Title = "Keybind",
		Default = Enum.KeyCode.X,
		Callback = function(value)
			print(value)
		end,
	});
	
	GeneralSection:AddTextbox({
		Title = "Textbox",
		Placeholder = "Placeholder",
		Callback = function(value)
			print(value)
		end,
	});
	
	GeneralSection:AddDropdown({
		Title = "Single Dropdown",
		Values = {"Value 1","Value 2","Value 3"},
		Default = 'Value 1',
		Callback = function(value)
			print(value)
		end,
	});
	
	GeneralSection:AddDropdown({
		Title = "Multi Dropdown",
		Values = {"Value 1","Value 2","Value 3","Value 4","Value 5"},
		Default = {"Value 1"},
		Multi = true,
		Callback = function(value)
			print(value)
		end,
	});
	
	GeneralSection:AddParagraph({
		Title = 'Paragraph',
		Content = "Hello sir\ni'm travit skot\ni need 2,000 dollars to get back to amareka\nsend paypal sir"
	})
end;


ExampleSection:AddToggle({
	Title = 'Auto Parry',
})

ExampleSection:AddToggle({
	Title = 'Auto Farm',
})

ExampleSection:AddToggle({
	Title = 'Accept Quest',
})

ExampleSection:AddToggle({
	Title = 'Auto Attack',
})

ExampleSection:AddToggle({
	Title = 'Auto KYS',
})

ExampleSection:AddToggle({
	Title = 'Auto Fuck',
})
```
