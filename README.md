# Discord Link Display GUI for Roblox

A modern, responsive Discord invite link display GUI for Roblox games with mobile and PC optimization.

## 🎨 Features

- ✨ **Modern Design** - Clean, Discord-themed UI with smooth animations
- 📱 **Mobile & PC Optimized** - Automatically detects platform and adjusts layout
- 📋 **Manual Copy Support** - Click textbox to select all text for easy copying
- 🎭 **Smooth Animations** - Professional fade-in/fade-out transitions
- 🎯 **Hover Effects** - Interactive button and input effects (PC only)
- 🔄 **Toggle Button** - Compact "DISCORD" button to show/hide the panel

## 📦 Installation

1. Open Roblox Studio
2. Navigate to **StarterGui**
3. Insert a **ScreenGui**
4. Insert a **Script** or **LocalScript** into the ScreenGui
5. Copy and paste the code into the script
6. Modify the Discord link in the configuration section

## ⚙️ Configuration

Edit the `CONFIG` table at the top of the script:

```lua
local CONFIG = {
    DiscordLink = "https://discord.gg/jRB3vn5gYF", -- Replace with your Discord link
    -- Colors and layout settings...
}
```

### Customizable Settings:
- **Discord Link** - Your Discord server invite link
- **Colors** - All UI colors (Discord theme, backgrounds, etc.)
- **Mobile Layout** - Button size, position, and text size for mobile
- **PC Layout** - Button size, position, and text size for PC

## 🎮 Usage

### For Players:
1. Click the **DISCORD** button at the top of the screen
2. The Discord link panel will appear below the button
3. Click the textbox to automatically select the entire link
4. Manually copy the link using your device's copy function:
   - **PC**: `Ctrl + C`
   - **Mobile**: Long press and select "Copy"

### Button Position:
- **Mobile**: Centered at top (Y position: -46)
- **PC**: Left-center position (X: 0.5, -230 | Y: -46)

## 📱 Platform Support

### Mobile
- Touch-optimized button size (65x25)
- Compact panel (160x60)
- Smaller text (11px)

### PC
- Mouse hover effects
- Slightly larger UI (70x30 button, 170x70 panel)
- Standard text (12px)

## 🎨 Visual Features

- **Toggle Button**: Discord-colored button with white outline
- **Panel**: Dark-themed container with Discord accent border
- **Link Box**: Selectable textbox with focus effects
- **Animations**: Smooth fade transitions for all elements

## 🔧 Technical Details

### Services Used:
- `Players` - Get local player
- `UserInputService` - Platform detection
- `TweenService` - Smooth animations

### Key Components:
- **ScreenGui** - Main container
- **TextButton** - Toggle button
- **Frame** - Panel container
- **TextBox** - Discord link input (editable for selection)

## 📝 Code Structure

```
1. Services & Configuration
2. Platform Detection
3. UI Creation (Button, Frame, TextBox)
4. Toggle Function with Animations
5. Event Handlers (Click, Focus, Hover)
6. Debug Output
```

## 🛠️ Customization Tips

1. **Change Colors**: Edit the `Colors` table in `CONFIG`
2. **Adjust Position**: Modify `Mobile` or `PC` position values
3. **Resize Elements**: Change size values in `Mobile` or `PC` tables
4. **Animation Speed**: Adjust `TweenInfo` values

## 📄 License

Free to use and modify. Credit appreciated but not required.

## 👤 Author

**ItoRenz00**

## 🐛 Known Issues

- None currently reported

## 📮 Support

For issues or questions, please join the Discord server or contact the author.

## 🔄 Version History

### v1.0.0 (Current)
- Initial release
- Mobile and PC optimization
- Manual copy support
- Smooth animations
- Modern Discord-themed design

---

**Made with ❤️ for the Roblox community**
