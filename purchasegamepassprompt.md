# Purchase gamepass prompt.
**Create a screen gui, add a button and a local script, put the script below in the local script.**

```
-- Scripted by flvffywvffy

local product = 22822715 --Replace ID with your Dev Product ID or Gamepass ID

local market = game:GetService("MarketplaceService")
local Players = game:GetService("Players")

script.Parent.Product.MouseButton1Click:Connect(function()
	local player = Players.LocalPlayer
	market:PromptProductPurchase(player,product) --If using Dev Product ID type "PromptProductPurchase" | If using Gamepass ID, type "PromptGamePassPurchase" 
end)
```

[Image](https://i.imgur.com/fHfDhyh.png)
