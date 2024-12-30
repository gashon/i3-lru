# i3-lru

A lightweight i3 window switcher based on LRU (Last Recently Used) order.

## Features

- **i3-lru-daemon**: Tracks window focus events to maintain LRU order.
- **i3-lru**: Displays a rofi menu for fast window switching.

## Requirements

- [rofi](https://github.com/davatorium/rofi)
- jq
- i3-wm (or compatible window manager)

## Installation

Install from the AUR:
```
yay -S i3-lru
```

## Usage

1. Start the daemon:
   ```
   i3-lru-daemon &
   ```
   (Optional: Use a systemd user service for auto-start.)

2. Open the switcher:
   ```
   i3-lru
   ```

Press **Tab** and **Enter** to quickly toggle between recent windows.

## License

MIT
