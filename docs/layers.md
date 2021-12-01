## Introduction
Seeing the need to compress files for smaller .iso/.img files, and to run Floflis in other platforms (routers, IoT, handheld gaming consoles): I had the idea of Floflis' Layers, which makes Floflis modular and lightweight.

Bellow are the layers explained:

### Recipes

Not a working layer, but it contains references of compilers (for any supported platform), source-codes and different build versions (such as Floflis DNA's Normal and Lite versions).

## DNA

<img src="../img/brand/1-dna.png">

The first and most lightweight layer, focused on weaker hardware (routers, IoT, etc). It is the building blocks for the upper layers and for the whole Floflis.

Includes:

* Floflis CLI
* Installer

Floflis `DNA` can upgrade to Floflis `Core` or just install need parts of it (as `Core` can install some features from `Soil`).

## Core

<img src="../img/brand/2-core.png">

Very lightweight, can run from an intermediary router to even an Nintendo DS. Focused on IoT devices. Totally based on CLI. Includes:

* Directory scheme (tree, /1 folder)
* Yggdrasil
* NodeJS?

### Server

Despite being listed as an layer to where `Core` can upgrade into, its an extension to Floflis Core.
The `Core` layer doesn't depends upon the `Server` layer to upgrade into `Soil`.

As the name suggests, this layer is focused on servers.

## Soil

<img src="../img/brand/3-soil.png">

Floflis Core can be upgraded to Soil layer, which contains:

* CLI web browser (elinks)
* CLI games
* Sounds
* Audio player

## Grass

<img src="../img/brand/4-grass.png">

Initially thought for Playstation 2. Contains a very basic UI (remembers Windows 1/3), although can render some graphics.

* IPFS (with improvements to be lightweight)?
* Ethereum system/APIs
* Aragon + APM?
* Dillo web browser
* Video player with audio player

IPFS and Aragon can be installed from Floflis `Core` or `DNA`.?

## Base

<img src="../img/brand/5-base.png">

A lightweight desktop version, thought to run on Windows NT/95 machines and above.

* Midori web browser (need to be compatible with Dillo browser)
* HTML5 apps (needs a lightweight webview that works on old devices)?
* Lightweight version of VLC Media Player

## Home

<img src="../img/brand/6-home.png">

For intermediary computers.

* Electron
* HTML5Apps Platform
* Firedoge web browser (need to be compatible with Midori browser)
* VLC Media Player?

## Ultimate

<img src="../img/brand/7-ultimate.png">

Contains all feature sets.

* Application layers/loaders (Windows, MacOS, Android)
* Advanced media softwares (video/audio composition/edit, DVD creation)
* others, from feature sets and packs

## Planetary

<img src="../img/brand/8-planetary.png">

No information, yet.

## Stellar

<img src="../img/brand/9-stellar.png">

No information, yet.

## Quantum (draft, outdated - new layers were added before)

<img src="../img/brand/10-quantum.png">

As Windows keeps with practically the same disk size, Floflis Quantum is here because OSes needs to continue evolving.

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
