# RIFT Client 1.0.0 Beta

RIFT is an independent Minecraft Java launcher project with original red-and-black branding.

## Current repository status

This repository is not yet a verified Windows release. The complete editable project is delivered separately as `RIFT-Client-v1.0.0-Beta-Source.zip` in the associated work session. No installer or game-launch result should be inferred from this README.

## Project direction

- Maintain one source root named `rift source/`.
- Keep the website source under `rift source/websitepro/`.
- Use a branded NSIS assisted setup with a selectable installation folder, Desktop and Start Menu shortcuts, and an uninstaller that preserves profiles/game data.
- Build Windows x64 on a Windows runner so Electron and NSIS dependencies are installed for the right platform.
- Fetch Minecraft versions and required game/runtime files only when needed; do not package the entire game ecosystem in the initial installer.
- Publish a stable release only after Windows installation, authentication, version installation, and actual game launch have been verified.

## Build source

Use the delivered source ZIP and run `client/BUILD-WINDOWS.bat` on Windows. Node.js and an active network connection to the npm registry are required. It runs the branding generator, project tests, and the Electron Builder NSIS packaging target.

## Beta disclaimer

Windows compilation and real Minecraft game launching have not been verified in this repository yet. Do not advertise a downloadable installer until the build artifact exists and passes Windows testing.