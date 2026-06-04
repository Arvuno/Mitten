[![CI](https://github.com/Arvuno/mitten/actions/workflows/ci.yml/badge.svg)](https://github.com/Arvuno/mitten/actions)
# Mitten
Infinite canvas drawing application.

## Showcase

![Showcase](./Images/showcase.gif)

## Builds

Grab the builds <https://apos.itch.io/mitten>.

## Controls

### Draw

| Action | Shortcut |
| --- | --- |
| Draw | Left click |
| Draw lines | Shift + Left click |
| Change brush size (drag left to shrink, right to increase) | Control + Shift + Left click |
| Select a different color | Alt + Hover |
| Select a different background color | Control + Alt + Hover |
| Toggle eraser | E |

### Camera

| Action | Shortcut |
| --- | --- |
| Drag the camera | Middle click |
| Zoom | Scroll wheel |
| Zoom (drag up to zoom in, down to zoom out) | Control + Middle click |
| Rotate | Dot and Comma |
| Hyper zoom (hold; release to go back) | Space |
| Save camera position | Control + 1, Control + 2, ... Control + 9 |
| Load saved camera position | 1, 2, ... 9 |
| Toggle between current and previous position | Mouse extra buttons |

### Misc

| Action | Shortcut |
| --- | --- |
| Undo | Control + Z |
| Redo | Control + Shift + Z |
| Undo everything | Control + Backspace |
| Redo everything | Control + Shift + Backspace |
| Toggle borderless fullscreen | F11 |
| Toggle fullscreen | Alt + Enter |
| Toggle mouse cursor visibility | M |

## Saved files

Saved next to the application's executable.

* Drawing.json - Your whole canvas is saved there including undo redo and camera position.
* Settings.json - Window settings are saved here. Includes if the app should start in fullscreen, vsync and fixed timestep.

## Restore

```
dotnet restore Platforms/DesktopGL
dotnet restore Platforms/WindowsDX
```

## Run

```
dotnet run --project Platforms/DesktopGL
dotnet run --project Platforms/WindowsDX
```

## Debug

In vscode, you can debug by pressing F5.

## Publish

```
dotnet publish Platforms/DesktopGL -c Release -r win-x64 --output artifacts/windows
dotnet publish Platforms/DesktopGL -c Release -r osx-x64 --output artifacts/osx
dotnet publish Platforms/DesktopGL -c Release -r linux-x64 --output artifacts/linux
```

```
dotnet publish Platforms/WindowsDX -c Release -r win-x64 --output artifacts/windowsdx
```
