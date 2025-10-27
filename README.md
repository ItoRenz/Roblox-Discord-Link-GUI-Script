# Discord Link Display GUI

A sleek and optimized Discord link display GUI for Roblox, supporting both Mobile and PC platforms with instant toggle and manual copy functionality.

## ✨ Features

- 🎨 **Modern Discord-themed Design** - Clean UI with Discord's signature colors
- 📱 **Cross-Platform Support** - Optimized layouts for both Mobile and PC
- ⚡ **Instant Toggle** - Zero-lag panel opening/closing with no animations
- 📋 **Manual Copy Support** - Easy text selection for copying Discord links
- 🎯 **Smooth Hover Effects** - Enhanced UX with button hover animations (PC only)
- 🔧 **Easy Configuration** - Simple setup with customizable Discord link

## 📦 Installation

1. **Download** the `DiscordLinkGui.lua` script
2. **Place** the script in `StarterPlayer > StarterPlayerScripts`
3. **Configure** your Discord link in the CONFIG section
4. **Test** in-game!

## ⚙️ Configuration

Edit the `CONFIG` table to customize your Discord link:

```lua
local CONFIG = {
    DiscordLink = "https://discord.gg/jRB3vn5gYF", -- Replace with your Discord link
    -- ... other settings
}
```

## 🎮 Usage

### For Players:
1. Click the **DISCORD** button to open the panel
2. Click the text box to select all text
3. Copy the Discord link manually (Ctrl+C / Cmd+C)
4. Click the button again to close the panel

### Platform Detection:
- **Mobile**: Smaller UI, touch-optimized
- **PC**: Larger UI with hover effects

## 🛠️ Technical Details

### Services Used:
- `Players` - Player management
- `UserInputService` - Platform detection
- `TweenService` - Smooth hover animations

### Key Features:
- **Instant Toggle**: No animation delays for optimal performance
- **Auto Platform Detection**: Automatically adjusts UI for Mobile/PC
- **Manual Copy**: Text selection support for easy copying
- **Persistent GUI**: `ResetOnSpawn = false` keeps GUI on respawn

## 📱 Platform Specifications

### Mobile:
- Toggle Button: 65x25 pixels
- Panel Size: 160x60 pixels
- Text Size: 11
- Touch-optimized positioning

### PC:
- Toggle Button: 70x30 pixels
- Panel Size: 170x70 pixels
- Text Size: 12
- Hover effects enabled

## 🎨 Color Scheme

- **Discord Blue**: `#5865F2` (88, 101, 242)
- **Discord Hover**: `#6776FF` (103, 118, 255)
- **Dark Background**: `#1E2124` (30, 33, 36)
- **Input Box**: `#282B30` (40, 43, 48)

## 📋 Requirements

- Roblox Studio
- Basic knowledge of LocalScripts
- A Discord server invite link

## 🚀 Performance

- **Zero Lag**: Instant panel toggle with no animations
- **Lightweight**: Minimal resource usage
- **Optimized**: Platform-specific configurations

## 📄 License

This project is open source and available for use in your Roblox games.

## 👤 Author

**ItoRenz00**

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

## ⭐ Support

If you like this project, please give it a star on GitHub!

---

**Note**: Replace the Discord link in the CONFIG section with your own server invite link before using in your game.
