## Introduction
Seeing the need to compress files for smaller .ISO file, and to run Floflis in other platforms (routers, IoT, handheld gaming consoles), I had the idea of Floflis' Layers, which makes Floflis modular and lightweight.

Bellow are the layers explained:

## Recipes

Not a working layer, but it contains references of compilers (for any supported platform) and source-codes.

## DNA

The most lightweight layer, focused on weaker hardware (routers, IoT, etc). It is the building blocks for the whole Floflis.
Includes:

* Floflis CLI
* Installer

Floflis `DNA` can upgrade to Floflis `Core` or just install need parts of it (and also from `Soil`).

## Core

Very lightweight, can run from a intermediary router to even a Nintendo DS. Focused on IoT devices. Totally based on CLI. Includes:

* Directory scheme (tree, /1 folder)
* CJDNS + Yggdrasil
* NodeJS
* Dat protocol

## Soil

Floflis Core can be upgraded to Soil layer, which contains:

* CLI web browser (elinks)
* CLI games
* Sounds
* Audio player

## Grass

Initially thought for Playstation 2. Contains a very basic UI (remembers Windows 1/3), although can render some graphics.

* IPFS (with improvements to be lightweight)
* Ethereum system/APIs
* Aragon + APM
* Dillo web browser
* Video player with audio player

IPFS and Aragon can be installed from Floflis `Core` or `DNA`.

## Base

A lightweight desktop version, thought to run on Windows NT/95 machines and above.

* Midori web browser (need to be compatible with Dillo browser)
* HTML5 apps (needs a lightweight webview that works on old devices)
* Lightweight version of VLC Media Player

## Home

For intermediary computers.

* Electron
* HTML5Apps Platform
* Firefox/Brave web browser (need to be compatible with Midori browser)
* VLC Media Player

## Ultimate

Contains all feature sets.

* Application layers/loaders (Windows, MacOS, Android)
* Advanced media softwares (video/audio composition/edit, DVD creation)
* others, from feature sets and packs

## Quantum

As Windows keeps with practically the same disk size, Floflis Quantum is because a OS needs evolution.

* Blu-ray as installation media, and comes with BD disk reader/creator software
* P2P server features
* Fancy, 3D animations
* Lots of transitions and effects

So, this is the dependence scheme, including layers:

```
BIOS/UEFI
  -- Unix/Firmware
     -- Linux kernel
        --Floflis DNA
          -- Floflis Core
             -- Floflis Soil
                -- BSD/GNU OS/Debian
                   -- Floflis Grass
                      -- Floflis Base
                         -- Floflis Home
                            -- Floflis Ultimate
                               -- Floflis Quantum
```

Blog posts about the introduction of Layers: [1](https://floflis.github.io/blog/2019/07/floflis-layers-recipe-core-substratum-base-ultimate/), [2](https://floflis.github.io/blog/2019/07/new-layers-for-floflis-dna-and-home/).