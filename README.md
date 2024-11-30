local Rayfield = loadstring(game:HttpGet('https://[Log in to view URL]'))()

local Window = Rayfield:CreateWindow({
   Name = "의문의hub",
   Icon = 0, -- Icon in Topbar. Can use Lucide Icons (string) or Roblox Image (number). 0 to use no icon (default).
   LoadingTitle = "기다려주세요...",
   LoadingSubtitle = "by 누군가",
   Theme = "Default", -- Check https://[Log in to view URL]

   DisableRayfieldPrompts = false,
   DisableBuildWarnings = false, -- Prevents Rayfield from warning when the script has a version mismatch with the interface

   ConfigurationSaving = {
      Enabled = true,
      FolderName = nil, -- Create a custom folder for your hub/game
      FileName = "Big Hub"
   },

   Discord = {
      Enabled = true, -- Prompt the user to join your Discord server if their executor supports it
      Invite = "https://[Log in to view URL]", -- The Discord invite code, do not include discord.gg/. E.g. discord.gg/ABCD would be ABCD
      RememberJoins = true -- Set this to false to make them join the discord every time they load it up
   },

   KeySystem = true, -- Set this to true to use our key system
   KeySettings = {
      Title = "키시스템",
      Subtitle = "기다려주세요",
      Note = "환영합니다 key=콩순이", -- Use this to tell the user how to get a key
      FileName = "콩순이", -- It is recommended to use something unique as other scripts using Rayfield may overwrite your key file
      SaveKey = true, -- The user's key will be saved, but if you change the key, they will be unable to use your script
      GrabKeyFromSite = true, -- If this is true, set Key below to the RAW site you would like Rayfield to get the key from
      Key = {"https://[Log in to view URL]"} -- List of keys that will be accepted by the system, can be RAW file links (pastebin, github etc) or simple strings ("hello","key22")
   }
})

local Tab = Window:CreateTab("프나펑", nil) -- Title, Image
local Section = Tab:CreateSection("메인")

Rayfield:Notify({
   Title = "로딩중",
   Content = "by 누군가",
   Duration = 2,
   Image = 4483362458,
})

local Button = Tab:CreateButton({
   Name = "오토플레이",
   Callback = function()
   loadstring(game:HttpGet("https://[Log in to view URL]"))()
   end,
})

local Tab = Window:CreateTab("가강전", nil) -- Title, Image
local Section = Tab:CreateSection("메인")

local Button = Tab:CreateButton({
   Name = "고죠(사이타마로실행)",
   Callback = function()
   loadstring(game:HttpGet("https://[Log in to view URL]"))()
   end,
})

local Tab = Window:CreateTab("배드워즈", nil) -- Title, Image
local Section = Tab:CreateSection("메인")

local Button = Tab:CreateButton({
   Name = "vape v4",
   Callback = function()
   loadstring(game:HttpGet("https://[Log in to view URL]", true))()
   end,
})

local Tab = Window:CreateTab("프리즌라이프", nil) -- Title, Image
local Section = Tab:CreateSection("메인")

local Button = Tab:CreateButton({
   Name = "킬아우라/차량소환등등",
   Callback = function()
   loadstring(game:HttpGet("https://[Log in to view URL]"))()
   end,
})
