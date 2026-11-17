# InvokerApp 2

**Version 2.0.0** is a Windows desktop app for managing Invoker spell layouts, the on-screen overlay, and custom spell combos.

Version 2 builds on the original overlay app with a native WinForms Combo Studio, Combo Assistant, configurable combo hotkeys, and an Arcane Premium interface.

## Download

Download the latest Windows build from [GitHub Releases](https://github.com/Melonvw/InvokerApp/releases/latest).

Extract the ZIP and run `InvokerApp.exe`. The framework-dependent build requires the **.NET 8 Desktop Runtime** for Windows.

Your settings are stored in `settings.json` beside the application. Keep this file when upgrading if you want to preserve layouts, combos, themes, and hotkeys.

## Features

- Starts in Combo Studio Home, with an explicit switch to Overlay mode.
- Three independently configurable spell layouts; press `Caps Lock` to cycle layouts.
- Edit spell hotkeys and reorder spell rows. Assigning a key already used by another spell swaps both bindings and rows.
- Combo library and editor with shared or layout-specific combos, ordered spell sequences, and drag-and-drop reordering.
- Combo Assistant with Manual and Automatic modes, progress, and Previous, Next, Pause, Resume, Reset, and Stop controls.
- Configurable global shortcuts for starting, advancing, and resetting a combo.
- Five themes, including Arcane Premium.

## Quick start

1. Launch `InvokerApp.exe`; Combo Studio opens on Home.
2. Select **Switch to Overlay Mode** to show the overlay. Select **COMBO STUDIO** on the overlay to return.
3. In Combo Studio, create and save a combo, then open Combo Assistant.
4. Configure the Start, Next, and Reset shortcuts in Settings.

For detailed setup and usage instructions, see the [Persian tutorial](./README_COMBO_BUILDER_FA.txt).

## Build from source

Requirements: Windows and the .NET 8 SDK.

```powershell
dotnet build InvokerApp.csproj -c Release
```

The project is a C# .NET 8 Windows Forms application. Spell artwork and the supplied Arcane background are copied to the build output.

## Notes

InvokerApp is an independent community project and is not affiliated with or endorsed by Valve Corporation or Dota 2. The application sends configured keystrokes to the currently active window; it cannot verify in-game results.
