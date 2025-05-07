# 🌀 exter-menu
**Custom UI Menu System Inspired by NoPixel 4.0** — Built for QBCore & ExterCore

`exter-menu` is a fully custom NUI menu system designed with a modern and clean user interface similar to NoPixel 4.0. It serves as a stylish replacement for the default `qb-menu`, offering a smoother and more intuitive experience.

---

## 📦 Features

- ✅ **NoPixel 4.0 inspired UI design**
- ✅ **Full mouse interaction via NUI**
- ✅ **Automatic icon support for QBCore items**
- ✅ **Smooth transitions and animations**
- ✅ **Flexible: supports client events, server events, commands, and custom actions**
- ✅ **Supports menu grouping and sorting**
- ✅ **Exportable functions for integration with other scripts**

---

## 📂 Installation

1. **Download and extract** this resource into your `resources/[exter]` folder.
2. Add the following to your `server.cfg`:
   ```cfg
   ensure qb-core
   ensure exter-menu
   ```
3. Ensure your server uses QBCore and has a valid shared items configuration.

---

## 📌 Usage

Use this client-side export to open the menu:

```lua
exports['exter-menu']:openMenu({
    {
        header = "Main Menu Title",
        txt = "Short description here",
        icon = "fa-solid fa-star",
        params = {
            event = "your:eventName",
            args = { key = "value" }
        }
    },
    {
        header = "Close",
        icon = "fa-solid fa-x",
        params = {
            action = "close"
        }
    }
})
```

### 🔁 Available Functions

| Function | Description |
|---------|-------------|
| `openMenu(data)` | Opens the menu with given entries |
| `closeMenu()` | Closes the menu |
| `showHeader(text)` | Displays a top-level header in the menu |

---

## 🧠 Menu Item Format

```lua
{
  header = "Main text",
  txt = "Optional smaller text",
  icon = "fa-solid fa-icon", -- FontAwesome 6 Icon
  params = {
    event = "event:name",
    args = {}, -- optional
    server = true/false,
    command = true/false,
    qbcommand = true/false,
    action = "close" -- to close the menu
  }
}
```

---

## 🎨 Credits

- Created by [Sobing (CLTRALTDELETE)](https://github.com/CtrlAltDelete4413)
- UI inspired by NoPixel 4.0
- Part of the [ExterFramework](https://github.com/ExterCore)

---

## 💬 Notes

- This script depends on `exter-core`
- For best results, use a screen resolution of **1280x720** or higher
- Not compatible with `qb-menu` — acts as a full replacement

---

## Original Design By
[nm1-Dev](https://github.com/nm1-Dev)

---
![mennnuuu](https://github.com/user-attachments/assets/3c61f964-5f2f-49da-83e3-ae135da8df6b)

---
# PREVIEW

## 📜 License

Released under the **MIT License** — free to use, modify, and distribute with proper attribution.
