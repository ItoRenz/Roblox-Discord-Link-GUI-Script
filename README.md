# Discord Link GUI for Roblox

A modern, responsive Discord invite link display GUI for Roblox games with mobile and PC optimization.

## ✨ Features

- **Modern Discord-themed Design** - Sleek UI matching Discord's branding colors
- **Cross-Platform Support** - Optimized layouts for both mobile and PC
- **Smooth Animations** - Professional fade-in/fade-out effects with TweenService
- **Manual Copy Support** - Auto-select text when clicking for easy copying
- **Compact Design** - Minimal screen space usage
- **Hover Effects** - Interactive feedback on PC (disabled on mobile for performance)
- **Persistent GUI** - ResetOnSpawn disabled to maintain visibility

## 📱 Platform Detection

The script automatically detects the player's platform and adjusts:
- Button positioning
- Text sizes
- Frame dimensions
- Hover effects (PC only)

## 🎨 Design Specifications

### Toggle Button
- Size: 70×30 pixels
- Position: Center-top, offset left 200px (PC) or 55px (Mobile)
- Color: Discord Blurple (#5865F2)
- Text: "DISCORD" in Gotham Bold

### Main Panel
- Size: 170×58 pixels (PC) / 160×60 pixels (Mobile)
- Background: Dark Discord Gray (#1E2124)
- Border: Discord Blurple with transparency
- Rounded corners: 12px radius

## 📥 Installation

### Method 1: Roblox Studio (Recommended)
1. Open Roblox Studio
2. Navigate to `StarterGui`
3. Add a new `ScreenGui`
4. Change name `ScreenGui` to `Discord`
5. Insert a new `LocalScript`
6. Copy and paste the entire script
7. Configure the Discord link (see Configuration section)
8. Test in Play mode

### Method 2: Command Bar
1. Open Command Bar in Studio (View > Command Bar)
2. Paste the script
3. Press Enter

## ⚙️ Configuration

Edit the Discord link at the top of the script:

```lua
local DISCORD_LINK = "https://discord.gg/jRB3vn5gYF" -- Replace with your Discord link
```

Replace `jRB3vn5gYF` with your Discord server's invite code.

## 🎯 Usage

### For Players
1. Click the **DISCORD** button at the top of the screen
2. Panel opens with the Discord invite link
3. Click the text box to auto-select the link
4. Copy manually (Ctrl+C on PC, long-press on mobile)
5. Paste into your browser or Discord app

### For Developers
- Place the script in `StarterGui > LocalScript`
- Customize colors by editing `Color3.fromRGB()` values
- Adjust positions using `UDim2` values
- Modify animation speeds in `TweenInfo.new()`

## 🔧 Customization Options

### Colors
```lua
-- Toggle Button
BackgroundColor3 = Color3.fromRGB(88, 101, 242) -- Discord Blurple

-- Frame
BackgroundColor3 = Color3.fromRGB(30, 33, 36) -- Dark Gray

-- Text Box
BackgroundColor3 = Color3.fromRGB(40, 43, 48) -- Lighter Gray
```

### Positioning
```lua
-- Toggle Button Position (PC)
toggleButton.Position = UDim2.new(0.5, -200, 0, -43)

-- Toggle Button Position (Mobile)
toggleButton.Position = UDim2.new(0.5, -55, 0, -43)
```

### Animation Timing
```lua
-- Main animation (open/close)
local tweenInfo = TweenInfo.new(0.25, Enum.EasingStyle.Quad, Enum.EasingDirection.Out)

-- Quick animations (hover effects)
local tweenInfoQuick = TweenInfo.new(0.15, Enum.EasingStyle.Sine, Enum.EasingDirection.InOut)
```

## 📋 Requirements

- Roblox Studio (latest version recommended)
- LocalScript in StarterGui
- FilteringEnabled compatible
- No external modules required

## 🐛 Known Issues

- None reported

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📝 License

This project is open source and available for free use in your Roblox games.

## 💡 Tips

- Test on both mobile and PC devices
- Ensure your Discord invite link is set to never expire
- Consider adding the link to your game description as backup
- Use a custom invite link for tracking purposes

## 📞 Support

If you encounter any issues or have questions:
1. Check the console for error messages (F9 in-game)
2. Verify the script is in the correct location
3. Ensure your Discord link is valid
4. Test in both Studio and published game

## 🎓 Credits

Created for the Roblox development community.

---

**Note:** This GUI does not automatically copy to clipboard due to Roblox security restrictions. Players must manually copy the link.
