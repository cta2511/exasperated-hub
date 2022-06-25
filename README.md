-- antiban script:
setfflag("DFStringCrashPadUploadToBacktraceToBacktraceBaseUrl", "")
setfflag("DFIntCrashUploadToBacktracePercentage", "0")
-- the rest of the hub:

local Mercury = loadstring(game:HttpGet("https://raw.githubusercontent.com/deeeity/mercury-lib/master/src.lua"))()

-- GUI:

local GUI = Mercury:Create{
    Name = "Mercury",
    Size = UDim2.fromOffset(600, 400),
    Theme = Mercury.Themes.Dark,
    Link = "https://coppaware.xyz"
}

GUI:Notification{
	Title = "Sub to Me",
	Text = "https://www.youtube.com/channel/UCbzJZa8hKoYXYRAWvNIYUhg/videos",
	Duration = 30,
	Callback = function() end
}

-- tabs:

local Tab = GUI:Tab{
	Name = "universal-scripts",
	Icon = "rbxassetid://8569322835"
}

-- buttons:

Tab:Button{
	Name = "Sword Reach",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/cta2511/Sword-Reach/main/README.md'))() end
}

Tab:Button{
	Name = "Piano Autoplayer (INSTRUCTIONS: https://controlc.com/3652c39f)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('loadstring(game:HttpGetAsync("https://raw.githubusercontent.com/richie0866/MidiPlayer/main/package.lua"))()'))() end
}

Tab:Button{
	Name = "Netless Bypass",
	Description = nil,
		Callback = function() for i,v in next, game:GetService("Players").LocalPlayer.Character:GetDescendants() do
    if v:IsA("BasePart") and v.Name ~="HumanoidRootPart" then 
    game:GetService("RunService").Heartbeat:connect(function()
    v.Velocity = Vector3.new(-30,0,0)
    end)
    end
    end
 
    game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "Notification";
        Text = "Netless Ran";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16; end
}

Tab:Button{
	Name = "Dex V4 Rework",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://gist.githubusercontent.com/DinosaurXxX/b757fe011e7e600c0873f967fe427dc2/raw/ee5324771f017073fc30e640323ac2a9b3bfc550/dark%2520dex%2520v4'))() end
}

Tab:Button{
	Name = "Chat Bypass (CAN GET YOU BANNED)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://the-shed.xyz/roblox/scripts/ChatBypass'))() end
}

Tab:Button{
	Name = "E to Fling (R6 only)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet("https://pastebin.com/raw/q3y5ZeY9"))() end
}

Tab:Button{
	Name = "Copy Peoples Messages",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/cta2511/copy-specific-peoples-messages/main/README.md'))() end
}

Tab:Button{
	Name = "Copy Everyones Messages",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/cta2511/copy-everyones-messages/main/README.md'))() end
}

Tab:Button{
	Name = "Telekinesis",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/cta2511/telekinesis/main/README.md'))() end
}

Tab:Button{
	Name = "Among Us (R6 Only)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/cta2511/among-us/main/README.md'))() end
}

Tab:Button{
	Name = "Rainbow King Anims",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/cta2511/fe-rainbow-king-anims/main/README.md'))() end
}

Tab:Button{
	Name = "Spy On Private Chats",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/cta2511/spy-on-priv-chats/main/README.md'))() end
}

Tab:Button{
	Name = "Background Autoclicker",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/cta2511/background-autoclicker/main/README.md'))() end
}

Tab:Button{
	Name = "Parkour v2 (CMDS: controlc.com/8b1445c1)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://pastebin.com/raw/1dup3HSe'))() end
}

Tab:Button{
	Name = "Nameless Animations",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/cta2511/nameless-animations/main/README.md)'))() end
}

Tab:Button{
	Name = "Hat Visualizer",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/xaxaxaxaxaxaxaxaxa/Ciazware/main/Hat-Visualizer)'))() end
}

Tab:Button{
	Name = "Achromatic",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/cta2511/achromatic/main/README.md'))() end
}

Tab:Button{
	Name = "Hats Spin Around You (CMDS: https://controlc.com/b14decfd)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/cta2511/achromatic/main/README.md'))() end
}

-- tabs:

local Tab = GUI:Tab{
	Name = "game-specific-scripts/hubs",
	Icon = "rbxassetid://8569322835"
}

-- buttons:

Tab:Button{
	Name = "3008 Anti-Cheat Bypass",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/cta2511/3008-Anti-Cheat-Bypass/main/README.md'))() end
}

Tab:Button{
	Name = "3008 Hub",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('sssss'))() end
}

Tab:Button{
	Name = "FE2 Tomato Hub",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/cta2511/FE2-Hub/main/README.md'))() end
}

Tab:Button{
	Name = "Undertale Last Reset All Items",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/nabhek/undertale-last-reset-all-weapons-bypass/main/script.lua'))() end
}

Tab:Button{
	Name = "Robot 64 100% Save (NO BONUS CONTENT)",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/cta2511/r64-100percent-file/main/README.md'))() end
}

Tab:Button{
	Name = "Robot 64 Hub",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://gist.githubusercontent.com/iiDk-the-actual/08b9710a138209cc09908a1d88b47a0a/raw/522928ad71041db75b2ed48b99f6c8999fffbeb8/rfthgfghgfh'))() end
}

Tab:Button{
	Name = "Blox Hunt GUI",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/cta2511/blox-hunt-gui/main/main'))() end
}

Tab:Button{
	Name = "Raise a Floppa 2 GUI",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/cta2511/raise-a-floppa-2/main/README.md'))() end
}

Tab:Button{
	Name = "Slap Battles GUI",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/dizyhvh/slap_battles_gui/main/0.lua'))() end
}

Tab:Button{
	Name = "RealZz Hub",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/RealZzHub/MainV2/main/Main.lua'))() end
}

Tab:Button{
	Name = "Friday Night Bloxxin Autoplayer",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/o5u3/Friday-Night-Bloxxin-Autoplayer/main/Script.lua'))() end
}

Tab:Button{
	Name = "Survive the Killers in Area 51 GUI",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/Ghostmode65/STK-Bo2/master/STK-Menus/v5/STKv5.txt'))() end
}

Tab:Button{
	Name = "Funky Friday Autoplayer",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/wally-rblx/funky-friday-autoplay/main/main.lua'))() end
}

Tab:Button{
	Name = "FE2 TAS Maker",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/SomeScripterInABasement/Fe2Tas/main/README.md'))() end
}

Tab:Button{
	Name = "CoffeeWare",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/cta2511/coffeeware-leaked-cracked/main/README.md'))() end
}

Tab:Button{
	Name = "CoppaWare (Get Premium .gg/Up5R8SBEff",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('loadstring(game:HttpGet("https://raw.githubusercontent.com/youngchongosreal/coppaware/main/coppaware.lua"))()
'))() end
}

Tab:Button{
	Name = "Fake System Messages",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/cta2511/fake-system-messages/main/README.md'))() end
}

Tab:Button{
	Name = "Eclipse Hub",
	Description = nil,
	Callback = function() loadstring(game:HttpGet('https://pastebin.com/raw/hUSWsaE1'))() end
}
