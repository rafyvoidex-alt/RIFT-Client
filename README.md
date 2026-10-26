# RIFT Client 1.0.0 Beta

This repository holds the build snapshot for the RIFT Client Windows x64 beta. The maintained, editable project is distributed as `RIFT-Client-v1.0.0-Beta-Source.zip` from the developer workspace; the versioned build snapshot in this repo is split into `source-bundle-00.b64` … `source-bundle-08.b64` so GitHub Actions can reconstruct it without losing binary branding assets.

## Build
Pushes to `main`, version tags, and manual workflow runs invoke a Windows runner. CI restores the source snapshot, regenerates the branded RC icon and NSIS artwork, runs the source/syntax checks, builds `RIFT-Setup-x64.exe`, and uploads the EXE plus SHA-256 metadata as a 14-day Actions artifact.

## Current status
This is an unreleased beta. Actual Windows installation, Microsoft sign-in, supported loader matrix, and a real Minecraft game launch still require Windows runtime validation. The website release manifest remains unpublished until those checks pass.

The source snapshot intentionally does not contain Minecraft game files or Java runtimes; those are downloaded on demand by the launcher library.