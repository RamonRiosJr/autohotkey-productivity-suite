AutoHotkey Productivity Suite

A curated collection of custom AutoHotkey (AHK) scripts designed to streamline common tasks, minimize repetitive actions, and supercharge your daily workflow on Windows. Each tool is built to be lightweight, modular, and easy to customize.

🚀 Included Tools

This suite currently includes four major components:

Dynamic Window Management: Automatically resize and position application windows based on customizable rules or hotkeys.

Smart Clipboard Enhancement: A powerful clipboard manager that provides history, search, and text-transformation capabilities.

Media Controller with Gestures: Control system volume and media playback using simple mouse gestures or custom hotkeys.

Task Automation Launcher: A central hub to launch programs, complex scripts, or sequences of actions with a single hotkey.

🔧 Installation & Setup

Install AutoHotkey: Download and install the latest version from autohotkey.com.

Clone the Suite:

git clone [https://github.com/RamonRiosJr/autohotkey-productivity-suite.git](https://github.com/RamonRiosJr/autohotkey-productivity-suite.git)


Run Your Desired Tools: Each script is standalone. You can:

Run a single tool: Navigate to its folder (e.g., 1-Window-Management) and double-click the .ahk script.

Combine tools: You can create your own Master.ahk script and use #include to load all the components you want to use at once.

; Example Master.ahk
#Include %A_ScriptDir%\1-Window-Management\window-manager.ahk
#Include %A_ScriptDir%\3-Media-Controller\media-controller.ahk


Add to Startup: Place a shortcut to your desired .ahk script in the Windows Startup folder (shell:startup) to run it automatically.

🛠️ Suite Components

1. Dynamic Window Management

Folder: 1-Window-Management/

Purpose: Stop manually dragging and resizing windows. This script provides hotkeys to instantly snap windows to predefined screen locations (e.g., left half, right half, top-right quadrant).

Example Hotkeys (Customize as needed):

Ctrl + Alt + Left: Snap active window to the left 50% of the screen.

Ctrl + Alt + Right: Snap active window to the right 50% of the screen.

Ctrl + Alt + Up: Maximize active window.

2. Smart Clipboard Enhancement

Folder: 2-Smart-Clipboard/

Purpose: Breaks the "one item at a time" limitation of the default clipboard. This tool gives you a searchable history of items you've copied.

Example Hotkeys (Customize as needed):

Ctrl + Shift + V: Open the clipboard history window.

Ctrl + Alt + C: Copy selected text and automatically strip its formatting.

3. Media Controller with Gestures

Folder: 3-Media-Controller/

Purpose: Control your music and system volume without ever leaving your current window.

Example Hotkeys & Gestures (Customize as needed):

Gestures: Hold Right-Click + move mouse Down to Play/Pause. Hold Right-Click + move mouse Left for Previous Track.

Hotkeys: Ctrl + F10 for Volume Down, Ctrl + F11 for Volume Up.

4. Task Automation Launcher

Folder: 4-Task-Launcher/

Purpose: A simple, fast launcher for your most common tasks, scripts, and programs, triggered by a single hotkey.

Example Hotkeys (Customize as needed):

Ctrl + Space: Open the launcher GUI.

From the launcher, type ps to launch Photoshop, work to open your standard work applications, or backup to run a custom backup script.
