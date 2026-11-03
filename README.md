# VLP Launcher

VLP Launcher is a private desktop launcher for Minecraft: Java Edition, built by and for a small group of friends who play together (the "VELDADELO PANA" group).

It is a hobby project in active development. It is not a commercial product, it is not publicly distributed, and it is not affiliated with, endorsed by, or associated with Mojang Studios or Microsoft.

## What it does

- Manages separate Minecraft installations ("instances"), each with its own version, mod loader, mods, configuration, worlds, and resource packs.
- Downloads official game files (client, libraries, and assets) from Mojang's public servers and verifies them with SHA-1 checksums.
- Downloads the Java runtime that each Minecraft version requires from Mojang's official runtime distribution.
- Installs the Fabric mod loader using Fabric's public metadata API.
- Lets players search for and install mods from Modrinth through Modrinth's public API, including required dependencies, and enable, disable, or remove them.
- Launches the game locally.
- Planned: group "events" with shared modpacks that stay in sync for all members.

## Authentication

VLP Launcher is intended to sign players in with the official Microsoft authentication flow (Microsoft account, Xbox Live, and the Minecraft services), so that only people who own Minecraft: Java Edition can play online.

- The launcher never asks for, receives, or stores Microsoft account passwords. Sign-in happens on Microsoft's own pages.
- It only reads the basic information needed to start the game (player name, UUID, and ownership check).
- Players can sign out at any time, which removes the stored session data from their own computer.
- Tokens are stored locally on the player's device only. Nothing is sent to any server operated by this project.

## Technology

Electron, React, TypeScript, and Vite. Instance data is stored locally on each player's computer.

## Audience and distribution

This launcher is made for a closed group of a few friends. It does not collect analytics, does not run advertising, and does not sell anything.

## Disclaimer

Minecraft is a trademark of Mojang Studios / Microsoft. This project does not distribute Minecraft game files itself; all game files are downloaded directly from Mojang's official servers.
