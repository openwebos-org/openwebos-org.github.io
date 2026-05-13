# OpenWebOS
An experimental OS-in-a-browser built entirely with HTML, CSS, and JavaScript. Runs client-side with no server dependencies.
## Try It
Open `beta.html` in a browser, or visit the hosted version at **[openwebos-org.github.io](https://openwebos-org.github.io/rc/rc-alpha)**.
## Features
### Desktop Environment
- **OOBE Setup** — First-run wizard: pick a wallpaper, accent color, create a user profile
- **Login Screen** — User avatar, password entry, live clock with date
- **Top Bar** — App menu, WiFi indicator, user menu with shutdown/restart/logout/switch user
- **Homescreen** — Just-type search bar, widget area (clock, weather, calendar, notes, battery, uptime)
- **Launcher / Dock** — Bottom dock with pinned apps, drag-to-rearrange, remove badge, homescreen button
- **App Drawer** — Grid of all installed apps with drag-to-dock support, folders, edit mode with wobble animation
### Window Management
- **Cards Overview** — Swipe up from bottom corners to see all open windows as cards. Gesture navigation on touch and trackpad. Spring-animated 60fps transitions.
- **Card Windows** — Draggable, resizable windows with macOS-style traffic light dots (close/minimize/fullscreen). Fullscreen mode fills the desktop.
- **Switch between Cards and Windows** — All in settings.
### Built-in Apps
| App | Description |
|-----|-------------|
| **Siri-ish** | AI assistant with chat UI, two modes (new/legacy). Ask questions, open apps, do math. 100% local. |
| **Terminal** | OWOTS (OpenWebOS Terminal Standard) shell: `ls`, `cd`, `cat`, `echo`, `pwd`, `whoami`, `neofetch`, `uptime`, `cal`, `clear`, `help`, `app` |
| **Files** | File manager with folder navigation, sizes, create/delete/rename, home/docs/downloads/pictures/music/video dirs |
| **Music** | Audio player with demo tracks, play/pause/next/prev, progress bar, shuffle |
| **Weather** | Live weather with temperature, conditions, humidity, wind speed, location |
| **Calculator** | Scientific calculator with history, keyboard support, operation chaining |
| **Clock** | Large analog-style digital clock with live date display |
| **Calendar** | Month view with navigation, today highlighting, other-month dimming |
| **Notes** | Sticky notes with add/remove, scrollable list |
| **Contacts** | Contact list with avatars, phone/email display |
| **Settings** | Wallpaper, accent color, dock, widgets, users, keyboard, language, about, Siri-ish mode toggle |
| **App Store** | Browse and install available apps |
### Persistence
- User profiles, settings, wallpaper, accent color, dock layout, widgets, files, notes, contacts all persist via `localStorage`
- App drawer order and dock pinned apps survive page reload
- Widget preference and positions are saved
### Recovery System (`recovery.html`)
A TWRP-style recovery environment for system maintenance:
- **Wipe** — Clear all data, format localStorage, factory reset, wipe cache, wipe dalvik (simulated)
- **Backup / Restore** — Export all OS data as JSON download, import from file
- **File System** — Browse stored files, view raw data, virtual device storage
- **Date & Time** — Timezone picker, date/time set, epoch display
- **Profiles** — View registered users, profile details, fingerprints
- **Developer** — Port detection, Chrome/non-Chrome detection, import/export tools
- **Boot** — Reboot to OS, reboot to recovery, view boot logs
## Tech Stack
- Vanilla JavaScript (no frameworks)
- CSS custom properties, flexbox, grid, backdrop-filter, animations
- `localStorage` for persistence
- Deployment-ready via GitHub Pages (drag-and-drop)
## License
Open source and licensed under the MIT license. See the [GitHub organization](https://github.com/openwebos-org).
