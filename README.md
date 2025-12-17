# Introduction

Classic App Switcher is a 🖱️ Mouse friendly application switcher for GNOME inspired by the classic Mac OS. The minimal design blends discreetly into the GNOME UI, providing a familiar workflow for users transitioning from macOS while respecting GNOME's design principles.

The extension places an app indicator (icon and title) on the panel showing the currently focused application. This serves as a helpful anchor on both single and multi-workspace setups, especially useful since GNOME removed window titles from the top bar.

### **Key Features:**

- Panel button shows the currently focused application and opens a menu with window management functions
- Lists running applications on the current workspace
- Easily hide an app and retrieve all of its open windows
- Hide all other apps/windows allowing you to focus on the active window
- Window count showing visible and hidden (or minimized) windows and apps
- Workspace-isolated behaviour for fluid multi-workspace workflows
- Panel Button Scroll - Scroll DOWN to toggle between focused application and most recent below. Scroll UP to cycle through open application stack in reverse order (back-to-front - requires at least 3x open apps!)
- Optional Mac OS style keyboard shortcut support! (details below)
- Complements native GNOME features (Activities, Dash, Dynamic Workspaces)

### **Design Philosophy:**

Classic App Switcher augments GNOME's existing workflow rather than replacing it. Unlike dock or taskbar extensions, it works *with* GNOME's full-screen launcher and Activities Overview, not against them.

#### **Best Experienced:**

- On vanilla GNOME with a clean default panel
- Without competing taskbar/dock extensions
- Embracing GNOME's unique interface paradigm
- Remember: The Dash is **NOT** a Dock!

#### **Built for:**

New users seeking familiarity and experienced users wanting enhanced lightweight app/window management.

### Keyboard Shortcuts

This extension provides optional Mac-style keyboard shortcuts for accessibility:

   - **Super+H** / **Super+U**: Hide current app / Unhide last hidden app
   - **Super+M** / **Alt+Super+M**: Minimize current window / Unminimize last minimized window
   - **Alt+Super+H**: Hide all other applications on the current workspace
   - **Alt+Super+U**: Show all hidden applications/windows ('Show All' in menu)
   - **Super+W**: Close the current window
   - **Super+Q**: Quit the current application

Keyboard Access to the list of running apps is handled by GNOME's built-in **Super+Tab** function which by default shows running apps from ALL workspaces, to limit this to the current workspace (to match the classic-app-switcher's behaviour) go to; GNOME Settings → Multitasking → App Switching and select 'Include apps from the current workspace only' - Activities and the Dash now act as ‘Mission-Control’ showing all running apps across all active workspaces, while each workspace operates in glorious isolation! 😎

**A Short Note About Keyboard Shortcuts** 

This extension temporarily repurposes two GNOME shortcuts while enabled: **Super+H** (originally "Hide window") → now hides the entire app & **Super+M** which is assigned by default to open the Notification list (although the official documented shortcut is **Super+V** as shown in GNOME Settings > Keyboard > View and Customize Shortcuts) being a duplication we have borrowed it for 'Minimize Window' to complement our provided shortcuts. GNOME provides a built-in Hide/Show All toggle using **Super+D** if you need to quickly clear/restore your entire workspace.

If you need notifications/calendar access via the keyboard, please use **Super+V** instead (it does the same thing) 🙃

All shortcuts are restored to default when you disable the extension!

## Known Issues

- **Screen reader:** May have issues on some GNOME 48 installations. Works correctly in GNOME 49+

- **Extension Preferences:** Header logo icon not being recolored in dark-mode on Gnome 47/48. Resolved in GNOME 49+

- **GNOME Shell 50** Support is temporarily disabled due to an upstream event handling regression affecting panel button clicks. This will be re-enabled once the issue is resolved in GNOME Shell stable releases.

##### **Notice:**

1. In order to display a symbolic icon in the panel indicator, developers must ensure they have included a symbolic version of their app-icon in their package. Missing icons will result in the default full-color Icon being displayed. If you spot an application that has a missing icon please reach out to their developers politely requesting they add one!

2. This extension will function perfectly well if you do not have the minimize button enabled for window management - though you may find it helpful to enable this via GNOME Tweaks for an enhanced experience, particularly if you tend to work with multiple windows and apps on a single workspace. Note: GNOME 47+ disables the minimize button by default, but it can easily be re-enabled.

## Installation

🌐 Classic App Switcher is available for download on the Official [GNOME Extensions](https://extensions.gnome.org/extension/8849/classic-app-switcher/) website.
