Seeing the need to compress files to make smaller .ISO file, and to run Floflis in other platforms (routers, IoT, handheld gaming consoles), I had the idea of Floflis’ Layers, which makes Floflis modular and lightweight.

Bellow are the layers explained:

## Recipe

Not a working layer, but it contains references of compilers (for any supported platform) and source-codes.

## DNA

The most lightweight layer, focused on the most weak hardware (routers, IoT, etc).
Includes:

* Floflis CLI
* Installer

Floflis `DNA` can upgrade to Floflis `Core` or just install need parts of it (and also from `Substratum`).

## Core

Very lightweight, can run from a intermediary router to even a Nintendo DS. Focused on IoT devices. Totally based on CLI. Includes:

* Directory scheme (tree, /1 folder)
* CLI web browser
* NodeJS
* CJDNS + Yggdrasil
* Dat protocol

## Substratum

Initially thought for Playstation 2. Contains a very basic UI (remembers Windows 1⁄3) that remembers a CLI, although can render some graphics.

* Dillo web browser
* IPFS
* Ethereum system/APIs
* Aragon + APM

IPFS and Aragon can be installed from Floflis `Core` or `DNA`.

## Base

A lightweight desktop version, thought to run on Windows NT/95 machines and above.

* Midori web browser (need to be compatible with Dillo browser)
* HTML5 apps (needs a lightweight webview that works on old devices)

## Home

For intermediary computers.

* Firefox web browser (need to be compatible with Midori browser)
* Media softwares (media player)

## Ultimate

Contains all feature sets.

* Application layers/loaders (Windows, MacOS, Android)
* Advanced media softwares (video/audio composition/edit)
* others, from feature sets and packs

So, this is the dependence scheme, including layers:

```
BIOS/UEFI
  -- Unix/Firmware
    -- Linux kernel
      --Floflis DNA
        -- Floflis Core
          -- BSD/GNU OS/Debian
            -- Floflis Substratum
              -- Cinnamon Desktop Environment
                -- Floflis Basic
                  -- Floflis Home
                    -- Floflis Ultimate
```

Blog posts about the introduction of Layers: [1](https://floflis.github.io/blog/2019/07/floflis-layers-recipe-core-substratum-base-ultimate/), [2](https://floflis.github.io/blog/2019/07/new-layers-for-floflis-dna-and-home/).
