# cloud client downloads

the launcher for cloud client, plus everything it needs to keep itself and its packs up to date. the source lives somewhere else, this repo only holds finished builds :)

## getting it

grab `Cloud.Client_<version>_x64-setup.exe` from the [latest launcher release](https://github.com/pluters/cloudclient-downloads/releases), run it, sign in with your microsoft account and press play. it installs per user, no admin needed, and keeps itself updated.

you need your own copy of minecraft java edition (game pass works too). the launcher downloads the game straight from mojang, it is never bundled here.

## what's in the packs

**fabric 1.21.11:** cloud client, fabric api, sodium, lithium, ferritecore, immediatelyfast, entity culling, more culling (+ cloth config), badoptimizations, dynamic fps, sodium extra, reese's sodium options, mod menu (+ placeholder api), continuity, nuit, nuit interop

**forge 1.8.9:** cloud client, optifine, entity culling, betterfps, memoryfix, phosphor

## what's in this repo

| path | what it is |
| --- | --- |
| `manifest.json` | the packs, pinned to exact files with sha512 hashes. the launcher reads it before every play |
| `manifest.json.sig` | its signature. the launcher refuses a manifest that isn't signed by our key |
| `launcher/latest.json` | where the launcher checks for its own updates |
| `files/` | the jars we host ourselves (see below) |

## credits and licenses

most mods are not hosted here at all, the launcher downloads them from their authors' own pages:

* from modrinth: fabric api, sodium, lithium, ferritecore, immediatelyfast, entity culling, more culling, cloth config, badoptimizations, dynamic fps, sodium extra, reese's sodium options, mod menu, placeholder api, continuity, nuit, nuit interop, phosphor (legacy)
* from github: [memoryfix](https://github.com/prplz/MemoryFix) by prplz

hosted here:

* **cloud client** by pluters, CC0
* **optifine** by sp614x, redistributed with permission. the official download is [optifine.net](https://optifine.net)
* **betterfps** by Guichaguri, LGPL 2.1, see `files/forge-1.8.9/BetterFps-LICENSE.txt`. source at [github.com/Guichaguri/BetterFps](https://github.com/Guichaguri/BetterFps)

minecraft is © mojang ab. not an official minecraft product, not approved by or associated with mojang or microsoft.
