if not game:IsLoaded() then
    game.Loaded:Wait()
end

print("🔄 Đang tải Blox Fruits Hub...")

-- Tải UI chính
local success, err = pcall(function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/USERNAME/BloxFruitsHub/main/Main.lua"))()
end)

if not success then
    warn("❌ Lỗi tải script: " .. tostring(err))
end
