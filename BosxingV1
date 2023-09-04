local a = game:GetService("Players").LocalPlayer.PlayerGui.Main.StyleShop.Spin.SpinButton.Button
local style = game:GetService("Players").LocalPlayer.PlayerGui.Main.StyleShop.Slots.Slot1.Main.StyleName
local b = game:GetService("Players").LocalPlayer.PlayerGui.Main.StyleShop.Spin.Price

local lock = {"HITMAN", "SLUGGER", "HAWK", "GHOST"}


local fireclick = function(button)
    firesignal(button.MouseButton1Down)
    firesignal(button.MouseButton1Up)
    firesignal(button.MouseButton1Down)
    firesignal(button.MouseButton1Up)
end


coroutine.wrap(function()
    loadstring(game:HttpGet("https://github.com/Bosszat/Boxing/blob/main/autocode", true))()
 
  --  while task.wait(0) do
        if not table.find(lock, style.Text) then
            if not b.Visible then
                fireclick(a)
                print("random")
                task.wait(12) 
             
               
            else
                print("Not Spin")
                game:shutdown()
            end
        else
            local requestfunc = syn and syn.request or http and http.request or http_request or fluxus and fluxus.request or request

            local Data = {
                ["embeds"] = {
                    {
                        ["title"] = "Username: " .. game:GetService("Players").LocalPlayer.Name,
                        ["color"] = 0000,
                        ["description"] = "```\n" .. game:GetService("Players").LocalPlayer.PlayerGui.Main.StyleShop.Slots.Slot1.Main.StyleName.Text .. "\n```",
                    }
                }
            }

            local req = requestfunc({
                Url = "https://discord.com/api/webhooks/1147518522134626384/ukxnPgwMRlwIwhOK0y3ajiYfG02V8-4w04oLwDoL9kkqkKJeZ2ynaoN9rolbe7_Edp_F",
                Method = "POST",
                Headers = {
                    ["content-type"] = "application/json"
                },
                Body = game:GetService("HttpService"):JSONEncode(Data)
            })

            game:shutdown()
        end
    --end
end)()
