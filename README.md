# Awesome Open Replicas [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of open-source reimplementations, reverse-engineered engines, decompilations and faithful replicas of commercial software, games, SaaS products and platforms.

Every few weeks someone ships an open-source version of something that used to be locked up: a 25-year-old Xbox game running natively on Linux and Android, a Rust rewrite of the Adobe suite, a clean-room engine for a classic RTS, a self-hosted stand-in for a SaaS tool you pay per seat for. This list tracks the ones that are real, maintained, and legitimately distributed.

*Last reviewed: 13 October 2026.*

**Legend**

| Tag | Meaning |
|-----|---------|
| 🔬 | Reverse-engineered or clean-room **reimplementation** (behaviour, protocol or engine recreated from the original) |
| 🧬 | **Decompilation** or static **recompilation** of an original binary, often with a native port |
| 🔁 | Functional open-source **replica / alternative** to a commercial product |
| 🤖 | Built largely with **AI coding agents** (quality and review practices vary; some communities reject these) |
| 🆕 | Released or hit a major milestone in **2026** |
| 📦 | Bring your own copy: you must supply legally owned original game data or assets |
| ⚠️ | **Not OSI open source** (source-available, fair-code, non-commercial or open-core with notable restrictions); read the licence |

---

## Contents

- [Latest: October 2026](#latest-october-2026)
- [AI-Built Suite Replicas (ArtCraft)](#ai-built-suite-replicas-artcraft)
- [Games: Halo](#games-halo)
- [Games: Native Ports from Decompilations](#games-native-ports-from-decompilations)
- [Games: Static Recompilations](#games-static-recompilations)
- [Games: Completed or Near-Complete Decompilations](#games-completed-or-near-complete-decompilations)
- [Games: Reimplemented Engines](#games-reimplemented-engines)
- [Games: Recompilation Toolchains and Trackers](#games-recompilation-toolchains-and-trackers)
- [Emulators](#emulators)
- [Operating Systems and Compatibility Layers](#operating-systems-and-compatibility-layers)
- [Mobile OS and Services](#mobile-os-and-services)
- [Firmware and Hardware](#firmware-and-hardware)
- [Protocol, Client and Server Reimplementations](#protocol-client-and-server-reimplementations)
- [Office and Productivity](#office-and-productivity)
- [Adobe and Creative Suite](#adobe-and-creative-suite)
- [Design Tools](#design-tools)
- [Streaming and Media (Netflix, Spotify, YouTube)](#streaming-and-media-netflix-spotify-youtube)
- [Communication (Slack, Discord, Zoom)](#communication-slack-discord-zoom)
- [Social Platforms](#social-platforms)
- [Business SaaS](#business-saas)
- [Developer Platforms](#developer-platforms)
- [AI Products](#ai-products)
- [Cybersecurity Tooling](#cybersecurity-tooling)
- [Watchlist: No Source or Unclear Licence Yet](#watchlist-no-source-or-unclear-licence-yet)
- [Other Lists and Trackers](#other-lists-and-trackers)
- [Staying Safe: Fake Ports and Malware Bait](#staying-safe-fake-ports-and-malware-bait)
- [Deliberately Excluded](#deliberately-excluded)
- [Legal Notes](#legal-notes)
- [Contributing](#contributing)

---

## Latest: October 2026

- **ArtCraft "Crafting Apps"** (30 Sep – 9 Oct): Rust rewrites of Photoshop, Illustrator, Premiere Pro, After Effects, Lightroom, InDesign, Acrobat, then Word, Excel, PowerPoint, AutoCAD and Pro Tools. Built with heavy use of Claude. [Details below.](#ai-built-suite-replicas-artcraft)
- **OpenCE** (late Sep): native Halo: Combat Evolved for Windows, Linux and Android, built on the Halo CE decompilation, with 128-player system link. [Details below.](#games-halo)
- **Super Smash Bros. Melee** decompilation reached 100% (7 Sep).
- **Super Mario Galaxy** native port ("Astrocore") announced by Luma's Workshop (29 Sep), not yet released.
- **Donkey Kong 64**, **Pilotwings 64** and **Paper Mario** native PC ports released (Sep).

## AI-Built Suite Replicas (ArtCraft)

Clean-room reimplementations written in Rust, running on macOS, Windows, Linux and in the browser (WebAssembly). All repos are MIT or Apache-2.0. The ArtCraft name and logos are trademarked, so forks must rebrand. All of these are **early alpha**; the author has said they are not close to ready. Official source: [github.com/storytold](https://github.com/storytold) and getartcraft.com only.

| Project | Replicates | Notes |
|---------|-----------|-------|
| [PhotoCraft](https://github.com/storytold/photocraft) 🔬🤖🆕 | Adobe Photoshop | First of the suite, public ~30 Sep 2026. |
| [VectorCraft](https://github.com/storytold/vectorcraft) 🔬🤖🆕 | Adobe Illustrator | |
| [FilmCraft](https://github.com/storytold/filmcraft) 🔬🤖🆕 | Adobe Premiere Pro | |
| [EffectCraft](https://github.com/storytold/effectcraft) 🔬🤖🆕 | Adobe After Effects | |
| [LightCraft](https://github.com/storytold/lightcraft) 🔬🤖🆕 | Adobe Lightroom | |
| [DesignCraft](https://github.com/storytold/designcraft) 🔬🤖🆕 | Adobe InDesign | |
| [PdfCraft](https://github.com/storytold/pdfcraft) 🔬🤖🆕 | Adobe Acrobat | |
| [WordCraft](https://github.com/storytold/wordcraft) 🔬🤖🆕 | Microsoft Word | Pre-alpha; claimed ~62% feature parity, limited real-world .docx testing. |
| [GridCraft](https://github.com/storytold/gridcraft) 🔬🤖🆕 | Microsoft Excel | In development. |
| [DeckCraft](https://github.com/storytold/deckcraft) 🔬🤖🆕 | Microsoft PowerPoint | Alpha. |
| [CADCraft](https://github.com/storytold/cadcraft) 🔬🤖🆕 | Autodesk AutoCAD | Early development. |
| [SoundCraft](https://github.com/storytold/soundcraft) 🔬🤖🆕 | Avid Pro Tools | Pre-alpha. |

Coverage: [Gizmodo](https://gizmodo.com/someone-vibe-coded-a-free-knockoff-of-adobe-creative-suite-2000823322), [The Register](https://www.theregister.com/software/2026/10/08/rust-upstart-reveals-reimplementation-of-microsoft-office-with-claude-on-coding-duty/5301952), [Phoronix](https://www.phoronix.com/news/Photocraft-Filmcraft-AI).

## Games: Halo

All require your own original Xbox disc image. 📦

| Project | Replicates | Notes |
|---------|-----------|-------|
| [OpenCE](https://github.com/OpenCommunityEdition/OpenCE) 🧬🆕📦 | Halo: Combat Evolved (Xbox) | Native port (SDL3/OpenGL) for Windows, Linux and Android arm64. 128-player system link, online play via invite links, co-op. Formerly "halo-ce-universal". Download builds from **this repo's Releases** only. |
| [punpckhdq/halo](https://github.com/punpckhdq/halo) 🧬🆕 | Halo: Combat Evolved | The upstream matching decompilation (Xbox build 2342) that OpenCE builds on. CC0. Work in progress. |
| [halo2-decompiled](https://github.com/kirklandsig/halo2-decompiled) 🧬🆕 | Halo 2 (Xbox) | Matching decompilation, early. Source only. |

Coverage: [Notebookcheck](https://www.notebookcheck.net/Halo-Combat-Evolved-gets-online-multiplayer-on-Anbernic-RG35XX-H-with-a-23-player-match-reported-at-up-to-60-fps.1419202.0.html).

## Games: Native Ports from Decompilations

All of these require you to provide your own original game files. 📦

| Project | Replicates | Notes |
|---------|-----------|-------|
| [Dusklight](https://github.com/TwilitRealm/dusklight) 🧬🆕📦 | The Legend of Zelda: Twilight Princess (GameCube) | Released as "Dusk" May 2026, renamed Dusklight in 1.2. CC0. Windows, macOS, Linux, Android, iOS, Steam Deck. |
| [Ship of Harkinian](https://github.com/HarbourMasters/Shipwright) 🧬📦 | Zelda: Ocarina of Time | The Harbour Masters port that kicked off the modern decomp-port wave. |
| [2 Ship 2 Harkinian](https://github.com/HarbourMasters/2ship2harkinian) 🧬📦 | Zelda: Majora's Mask | Harbour Masters. |
| [Ghostship](https://github.com/HarbourMasters/Ghostship) 🧬🆕📦 | Super Mario 64 | Harbour Masters port; 1.0 Jan 2026, 2.0 May 2026. |
| [PaperBoat](https://github.com/HarbourMasters/PaperBoat) 🧬🆕📦 | Paper Mario | Harbour Masters, Sep 2026. |
| [Lighthouse](https://github.com/HarbourMasters/Lighthouse) 🧬🆕📦 | Banjo-Kazooie | Harbour Masters, Aug 2026 (discloses AI assistance). |
| [Starship](https://github.com/HarbourMasters/Starship) 🧬📦 | Star Fox 64 | Harbour Masters. |
| [SpaghettiKart](https://github.com/HarbourMasters/SpaghettiKart) 🧬📦 | Mario Kart 64 | Harbour Masters, custom tracks. |
| [sm64coopdx](https://github.com/coop-deluxe/sm64coopdx) 🧬📦 | Super Mario 64 | Online co-op. |
| [Perfect Dark port](https://github.com/fgsfdsfgs/perfect_dark) 🧬📦 | Perfect Dark (N64) | |
| [RSDKv5 Decompilation](https://github.com/RSDKModding/RSDKv5-Decompilation) 🧬📦 | Sonic Mania's engine | |
| [OpenGOAL](https://github.com/open-goal/jak-project) 🧬📦 | Jak and Daxter series (PS2) | Recreates Naughty Dog's GOAL compiler. |
| [REDRIVER2](https://github.com/OpenDriver2/REDRIVER2) 🧬📦 | Driver 2 (PS1) | |
| [Zelda3](https://github.com/snesrev/zelda3) 🔬📦 | Zelda: A Link to the Past (SNES) | C reimplementation. |
| [SAT-R sa2](https://github.com/SAT-R/sa2) 🧬📦 | Sonic Advance 2 (GBA) | Playable, unfinished. |
| [PsyDoom](https://github.com/BodbDearg/PsyDoom) 🔬📦 | PlayStation Doom | |
| [GeneralsGameCode](https://github.com/TheSuperHackers/GeneralsGameCode) 🔁 | C&C Generals / Zero Hour | Community fixes on the EA-released GPL source. |

## Games: Static Recompilations

Translate the original binary straight to native code, without a full decompilation. 📦

| Project | Replicates | Notes |
|---------|-----------|-------|
| [Zelda64Recomp](https://github.com/Zelda64Recomp/Zelda64Recomp) 🧬📦 | Zelda: Majora's Mask | The project that popularised N64Recomp. |
| [BanjoRecomp](https://github.com/BanjoRecomp/BanjoRecomp) 🧬🆕📦 | Banjo-Kazooie | GPL-3.0, Jan 2026. |
| [DK64 Rekongpiled](https://github.com/Rainchus/Donkey-Kong-64-Recompiled) 🧬🆕📦 | Donkey Kong 64 | GPL-3.0, Sep 2026. Advertised as made without generative AI. |
| [UnleashedRecomp](https://github.com/hedge-dev/UnleashedRecomp) 🧬📦 | Sonic Unleashed (Xbox 360) | |
| [Bluewake](https://github.com/chrissotraidis/bluewake) 🧬🆕📦 | Zelda: The Wind Waker (GameCube) | GPL-3.0; targets iPhone/iPad. |

## Games: Completed or Near-Complete Decompilations

Source reconstructions with no official native port yet.

| Project | Replicates | Status |
|---------|-----------|--------|
| [doldecomp/melee](https://github.com/doldecomp/melee) 🧬🆕 | Super Smash Bros. Melee | 100% matched, Sep 2026. |
| [projectPiki/pikmin](https://github.com/projectPiki/pikmin) 🧬🆕 | Pikmin (GameCube) | 100% matched, Jul 2026. |
| [zeldaret/tp](https://github.com/zeldaret/tp) 🧬 | Zelda: Twilight Princess | Basis for Dusklight. |
| [zeldaret/tww](https://github.com/zeldaret/tww) 🧬 | Zelda: The Wind Waker | In progress. |
| [n64decomp/sm64](https://github.com/n64decomp/sm64) 🧬 | Super Mario 64 | Complete; basis for most SM64 ports. |

## Games: Reimplemented Engines

Engine rewrites that read the original data files. 📦 unless stated.

| Project | Replicates | Notes |
|---------|-----------|-------|
| [OpenCaptive](https://github.com/yeager/OpenCaptive) 🔬🆕📦 | Captive (1990) / Liberation: Captive 2 | C/SDL3, extensive disassembly docs. |
| [OpenRA](https://github.com/OpenRA/OpenRA) 🔬 | Command & Conquer, Red Alert, Dune 2000 | |
| [Vanilla Conquer](https://github.com/TheAssemblyArmada/Vanilla-Conquer) 🔬📦 | C&C Tiberian Dawn / Red Alert | Portable builds of the EA-released source. |
| [OpenSAGE](https://github.com/OpenSAGE/OpenSAGE) 🔬📦 | EA SAGE engine (C&C Generals, BFME) | |
| [OpenMW](https://openmw.org) 🔬📦 | The Elder Scrolls III: Morrowind | |
| [Daggerfall Unity](https://github.com/Interkarma/daggerfall-unity) 🔬📦 | The Elder Scrolls II: Daggerfall | |
| [OpenTTD](https://github.com/OpenTTD/OpenTTD) 🔬 | Transport Tycoon Deluxe | Free replacement assets included. |
| [OpenRCT2](https://github.com/OpenRCT2/OpenRCT2) 🔬📦 | RollerCoaster Tycoon 2 | |
| [OpenLoco](https://github.com/OpenLoco/OpenLoco) 🔬📦 | Chris Sawyer's Locomotion | |
| [CorsixTH](https://github.com/CorsixTH/CorsixTH) 🔬📦 | Theme Hospital | |
| [DevilutionX](https://github.com/diasurgical/devilutionX) 🔬📦 | Diablo / Hellfire | |
| [fheroes2](https://github.com/ihhub/fheroes2) 🔬📦 | Heroes of Might and Magic II | |
| [VCMI](https://github.com/vcmi/vcmi) 🔬📦 | Heroes of Might and Magic III | |
| [OpenEnroth](https://github.com/OpenEnroth/OpenEnroth) 🔬📦 | Might and Magic VI–VIII | |
| [Julius](https://github.com/bvschaik/julius) / [Augustus](https://github.com/Keriew/augustus) 🔬📦 | Caesar III | |
| [OpenXcom](https://github.com/OpenXcom/OpenXcom) 🔬📦 | UFO: Enemy Unknown / X-COM: TFTD | |
| [Arx Libertatis](https://github.com/arx/ArxLibertatis) 🔬📦 | Arx Fatalis | |
| [OpenClaw](https://github.com/pjasicek/OpenClaw) 🔬📦 | Captain Claw (1997) | |
| [OpenLara](https://github.com/XProger/OpenLara) 🔬📦 | Tomb Raider (1996) | |
| [ScummVM](https://github.com/scummvm/scummvm) 🔬📦 | LucasArts, Sierra and hundreds of adventure games | |
| [OpenJK](https://github.com/JACoders/OpenJK) 🔬📦 | Jedi Academy / Jedi Outcast | |
| [ioquake3](https://github.com/ioquake/ioq3) 🔬📦 | Quake III Arena | |

## Games: Recompilation Toolchains and Trackers

| Project | What it does |
|---------|--------------|
| [N64Recomp](https://github.com/N64Recomp/N64Recomp) | N64 static recompiler; basis for most "Recomp" ports. |
| [XenonRecomp](https://github.com/hedge-dev/XenonRecomp) | Xbox 360 PowerPC static recompiler. |
| [ReXGlue SDK](https://github.com/rexglue/rexglue-sdk) 🆕 | Xbox 360 recompilation runtime built on XenonRecomp and Xenia; now behind most new 360 ports. Check licence. |
| [PS2Recomp](https://github.com/ran-j/PS2Recomp) 🆕 | Experimental PS2 static recompiler (GPL-3.0). |
| [ps3recomp](https://github.com/sp00nznet/ps3recomp) 🆕 | PS3 static recompiler (MIT). |
| [PSXRecomp](https://github.com/mstan/psxrecomp) 🆕⚠️ | PS1 static recompiler. PolyForm Noncommercial licence. |
| [decomp.dev](https://decomp.dev) | Progress tracker for decompilation projects. |
| [Read Only Memo: decomp list](https://readonlymemo.com/decompilation-projects-and-n64-recompiled-list) | Regularly updated list of decomps, recomps and finished ports. |

## Emulators

| Project | Replicates |
|---------|-----------|
| [Dolphin](https://github.com/dolphin-emu/dolphin) 🔬 | GameCube / Wii |
| [Cemu](https://github.com/cemu-project/Cemu) 🔬 | Wii U |
| [Eden](https://git.eden-emu.dev/eden-emu/eden) 🔬🆕 | Nintendo Switch (yuzu continuation, hosted off GitHub) |
| [Azahar](https://github.com/azahar-emu/azahar) 🔬 | Nintendo 3DS (Citra + Lime3DS merger) |
| [melonDS](https://github.com/melonDS-emu/melonDS) 🔬 | Nintendo DS |
| [PCSX2](https://github.com/PCSX2/pcsx2) 🔬 | PlayStation 2 |
| [RPCS3](https://github.com/RPCS3/rpcs3) 🔬 | PlayStation 3 |
| [shadPS4](https://github.com/shadps4-emu/shadPS4) 🔬 | PlayStation 4 |
| [PPSSPP](https://github.com/hrydgard/ppsspp) 🔬 | PSP |
| [Vita3K](https://github.com/Vita3K/Vita3K) 🔬 | PlayStation Vita |
| [xemu](https://github.com/xemu-project/xemu) 🔬 | Original Xbox |
| [Xenia Canary](https://github.com/xenia-canary/xenia-canary) 🔬 | Xbox 360 (where most [Xenia](https://github.com/xenia-project/xenia) development now happens) |
| [ares](https://github.com/ares-emulator/ares) 🔬 | Multi-system, accuracy-focused |
| [MAME](https://github.com/mamedev/mame) 🔬 | Arcade and thousands of other machines |
| [RetroArch](https://github.com/libretro/RetroArch) 🔬 | Multi-system frontend (libretro cores) |

> DuckStation (PS1) is excellent but is licensed CC BY-NC-ND, so it's not open source. Many Switch emulator forks were removed by DMCA in 2026 and are not listed.

## Operating Systems and Compatibility Layers

| Project | Replicates |
|---------|-----------|
| [ReactOS](https://github.com/reactos/reactos) 🔬 | Windows NT (binary-compatible OS) |
| [Wine](https://gitlab.winehq.org/wine/wine) 🔬 | Win32 API on Linux/macOS |
| [Proton](https://github.com/ValveSoftware/Proton) 🔬 | Wine + DXVK for Windows games on Linux |
| [Darling](https://github.com/darlinghq/darling) 🔬 | macOS userland on Linux |
| [Haiku](https://github.com/haiku/haiku) 🔬 | BeOS |
| [AROS](https://github.com/aros-development-team/AROS) 🔬 | AmigaOS 3.1 API |
| [Asahi Linux](https://asahilinux.org) 🔬 | Reverse-engineered drivers for Apple Silicon (M3 support official Sep 2026) |
| [FEX](https://github.com/FEX-Emu/FEX) 🔬 | x86/x86-64 on Arm64 Linux, à la Rosetta 2 |
| [Box64](https://github.com/ptitSeb/box64) 🔬 | x86-64 userspace on ARM64 / RISC-V / LoongArch |
| [Waydroid](https://github.com/waydroid/waydroid) 🔁 | Android apps on Linux, à la Windows Subsystem for Android |
| [xtool](https://github.com/xtool-org/xtool) 🔬 | Xcode build tooling on Linux/Windows |

## Mobile OS and Services

| Project | Replicates |
|---------|-----------|
| [microG](https://github.com/microg/GmsCore) 🔬 | Google Play Services |
| [GrapheneOS](https://github.com/GrapheneOS) 🔁 | Stock Android (hardened) |
| [LineageOS](https://lineageos.org) 🔁 | Vendor Android ROMs |

## Firmware and Hardware

| Project | Replicates |
|---------|-----------|
| [coreboot](https://review.coreboot.org/coreboot.git) 🔁 | Proprietary BIOS/UEFI firmware |
| [Valetudo](https://github.com/Hypfer/Valetudo) 🔬 | Robot vacuum vendor clouds (local-only control) |
| [Rockbox](https://www.rockbox.org) 🔁 | iPod and portable audio player firmware |

## Protocol, Client and Server Reimplementations

| Project | Replicates |
|---------|-----------|
| [Headscale](https://github.com/juanfont/headscale) 🔬 | Tailscale coordination server |
| [Vaultwarden](https://github.com/dani-garcia/vaultwarden) 🔬 | Bitwarden server API |
| [Samba](https://github.com/samba-team/samba) 🔬 | Windows SMB and Active Directory |
| [librespot](https://github.com/librespot-org/librespot) 🔬 | Spotify Connect client (Premium required) |
| [NewPipe](https://github.com/TeamNewPipe/NewPipe) 🔬 | YouTube Android client |
| [FreeTube](https://github.com/FreeTubeApp/FreeTube) 🔬 | YouTube desktop client |
| [BlueBubbles](https://github.com/BlueBubblesApp/bluebubbles-app) 🔬 | iMessage on Android, Windows, Linux (needs a Mac relay) |
| [mautrix-whatsapp](https://github.com/mautrix/whatsapp) 🔬 | WhatsApp protocol bridge for Matrix |
| [Minestom](https://github.com/Minestom/Minestom) 🔬 | Minecraft server, no Mojang code |
| [TrinityCore](https://github.com/TrinityCore/TrinityCore) 🔬 | World of Warcraft server |
| [AzerothCore](https://github.com/azerothcore/azerothcore-wotlk) 🔬 | World of Warcraft 3.3.5a server |
| [LandSandBoat](https://github.com/LandSandBoat/server) 🔬 | Final Fantasy XI server |

## Office and Productivity

See also WordCraft, GridCraft and DeckCraft in [ArtCraft](#ai-built-suite-replicas-artcraft).

| Project | Replicates |
|---------|-----------|
| [LibreOffice](https://github.com/LibreOffice/core) 🔁 | Microsoft Office |
| [ONLYOFFICE Docs](https://github.com/ONLYOFFICE/DocumentServer) 🔁 | Microsoft 365 / Google Docs |
| [Euro-Office](https://github.com/Euro-Office) 🔁🆕 | Microsoft 365 web editors. ONLYOFFICE fork backed by IONOS and Nextcloud; stable since Jun 2026. |
| [Collabora Online](https://github.com/CollaboraOnline/online) 🔁 | Office for the web |
| [Casual Office Sheets](https://github.com/CasualOffice/sheets) 🔁🆕 | Excel Online / Google Sheets (also Docs and Slides repos) |
| [CryptPad](https://github.com/cryptpad/cryptpad) 🔁 | Google Docs, end-to-end encrypted |
| [AppFlowy](https://github.com/AppFlowy-IO/AppFlowy) 🔁 | Notion |
| [AFFiNE](https://github.com/toeverything/AFFiNE) 🔁 | Notion + Miro |
| [Anytype](https://github.com/anyproto/anytype-ts) 🔁⚠️ | Notion, local-first (Any Source Available License) |
| [Outline](https://github.com/outline/outline) 🔁⚠️ | Confluence / Notion wiki (BSL 1.1) |
| [Docmost](https://github.com/docmost/docmost) 🔁 | Confluence |
| [Joplin](https://github.com/laurent22/joplin) 🔁 | Evernote |
| [Logseq](https://github.com/logseq/logseq) 🔁 | Roam Research |
| [Excalidraw](https://github.com/excalidraw/excalidraw) 🔁 | Whiteboard tools |
| [Stirling-PDF](https://github.com/Stirling-Tools/Stirling-PDF) 🔁 | Adobe Acrobat (open-core) |
| [Nextcloud](https://github.com/nextcloud/server) 🔁 | Dropbox / Google Drive / Microsoft 365 |
| [Immich](https://github.com/immich-app/immich) 🔁 | Google Photos / iCloud Photos |
| [Cal.com](https://github.com/calcom/cal.com) 🔁 | Calendly |
| [Documenso](https://github.com/documenso/documenso) 🔁 | DocuSign |

## Adobe and Creative Suite

See also the seven Adobe replicas in [ArtCraft](#ai-built-suite-replicas-artcraft).

| Project | Replicates |
|---------|-----------|
| [GIMP](https://gitlab.gnome.org/GNOME/gimp) 🔁 | Photoshop |
| [Krita](https://invent.kde.org/graphics/krita) 🔁 | Photoshop (painting) / Clip Studio |
| [Graphite](https://github.com/GraphiteEditor/Graphite) 🔁 | Photoshop + Illustrator, node-based |
| [Inkscape](https://gitlab.com/inkscape/inkscape) 🔁 | Illustrator |
| [Scribus](https://github.com/scribusproject/scribus) 🔁 | InDesign |
| [darktable](https://github.com/darktable-org/darktable) 🔁 | Lightroom |
| [RawTherapee](https://github.com/Beep6581/RawTherapee) 🔁 | Camera Raw / Lightroom |
| [Kdenlive](https://invent.kde.org/multimedia/kdenlive) 🔁 | Premiere Pro |
| [Shotcut](https://github.com/mltframework/shotcut) 🔁 | Premiere Pro |
| [Olive](https://github.com/olive-editor/olive) 🔁 | Premiere Pro (alpha, being restructured) |
| [Natron](https://github.com/NatronGitHub/Natron) 🔁 | After Effects / Nuke compositing |
| [Synfig](https://github.com/synfig/synfig) 🔁 | Adobe Animate |
| [Blender](https://projects.blender.org/blender/blender) 🔁 | Maya / Cinema 4D |
| [Audacity](https://github.com/audacity/audacity) 🔁 | Audition |
| [Ardour](https://github.com/Ardour/ardour) 🔁 | Pro Tools / Audition multitrack |
| [OBS Studio](https://github.com/obsproject/obs-studio) 🔁 | Commercial streaming / screen capture |

> Photopea and Affinity are free but not open source, so they are not listed.

## Design Tools

| Project | Replicates |
|---------|-----------|
| [Penpot](https://github.com/penpot/penpot) 🔁 | Figma / Adobe XD |
| [OpenPencil](https://github.com/open-pencil/open-pencil) 🔁🆕 | Figma (reads and writes .fig files) |
| [Doory](https://github.com/shaongitbd/doory) 🔁🆕 | Canva (self-hosted; launched on Show HN Oct 2026) |
| [Open Design](https://github.com/nexu-io/open-design) 🔁🆕 | Claude Design |

## Streaming and Media (Netflix, Spotify, YouTube)

| Project | Replicates |
|---------|-----------|
| [Jellyfin](https://github.com/jellyfin/jellyfin) 🔁 | Netflix-style experience for your own library (and Plex/Emby) |
| [Kyoo](https://github.com/zoriya/kyoo) 🔁 | Netflix-style self-hosted streaming server |
| [Kodi](https://github.com/xbmc/xbmc) 🔁 | Media centre / smart TV UI |
| [MediaCMS](https://github.com/mediacms-io/mediacms) 🔁 | Video hosting CMS |
| [PeerTube](https://github.com/Chocobozzz/PeerTube) 🔁 | YouTube (federated) |
| [Owncast](https://github.com/owncast/owncast) 🔁 | Twitch |
| [Navidrome](https://github.com/navidrome/navidrome) 🔁 | Spotify for your own music |
| [Audiobookshelf](https://github.com/advplyr/audiobookshelf) 🔁 | Audible |
| [Clone-Wars](https://github.com/GorvGoyl/Clone-Wars) 🔁 | 100+ UI clones of Netflix, Spotify, YouTube, Airbnb and more (learning projects) |

> Most "Netflix clones" are portfolio front-ends on the TMDB API. Anything that streams content you don't have rights to (torrent front-ends, embed scrapers) is excluded. See [Deliberately Excluded](#deliberately-excluded).

## Communication (Slack, Discord, Zoom)

| Project | Replicates |
|---------|-----------|
| [Mattermost](https://github.com/mattermost/mattermost) 🔁⚠️ | Slack (open-core; free tier tightened in v11) |
| [Rocket.Chat](https://github.com/RocketChat/Rocket.Chat) 🔁 | Slack |
| [Zulip](https://github.com/zulip/zulip) 🔁 | Slack (threaded) |
| [Stoat (formerly Revolt)](https://github.com/stoatchat) 🔁 | Discord. Renamed Oct 2025 after a trademark notice. |
| [Element](https://github.com/element-hq/element-web) 🔁 | Slack / Discord / Teams on Matrix |
| [Jitsi Meet](https://github.com/jitsi/jitsi-meet) 🔁 | Zoom / Google Meet |
| [BigBlueButton](https://github.com/bigbluebutton/bigbluebutton) 🔁 | Zoom for education |

## Social Platforms

| Project | Replicates |
|---------|-----------|
| [Mastodon](https://github.com/mastodon/mastodon) 🔁 | Twitter / X |
| [Lemmy](https://github.com/LemmyNet/lemmy) 🔁 | Reddit |
| [Pixelfed](https://github.com/pixelfed/pixelfed) 🔁 | Instagram |
| [Discourse](https://github.com/discourse/discourse) 🔁 | Forums / community platforms |
| [Ghost](https://github.com/TryGhost/Ghost) 🔁 | Substack / Medium |

## Business SaaS

| Project | Replicates |
|---------|-----------|
| [Plane](https://github.com/makeplane/plane) 🔁 | Jira / Linear |
| [Huly](https://github.com/hcengineering/platform) 🔁 | Linear + Slack + Notion |
| [Planka](https://github.com/plankanban/planka) 🔁⚠️ | Trello (fair-code licence) |
| [WeKan](https://github.com/wekan/wekan) 🔁 | Trello |
| [Twenty](https://github.com/twentyhq/twenty) 🔁 | Salesforce / HubSpot CRM |
| [Odoo Community](https://github.com/odoo/odoo) 🔁 | NetSuite / SAP Business One |
| [ERPNext](https://github.com/frappe/erpnext) 🔁 | NetSuite / SAP |
| [Baserow](https://github.com/baserow/baserow) 🔁 | Airtable (MIT core) |
| [Teable](https://github.com/teableio/teable) 🔁 | Airtable |
| [NocoDB](https://github.com/nocodb/nocodb) 🔁⚠️ | Airtable (Sustainable Use License) |
| [Chatwoot](https://github.com/chatwoot/chatwoot) 🔁 | Intercom / Zendesk |
| [Formbricks](https://github.com/formbricks/formbricks) 🔁 | Typeform / Qualtrics |
| [Metabase](https://github.com/metabase/metabase) 🔁 | Tableau / Looker |
| [Apache Superset](https://github.com/apache/superset) 🔁 | Tableau / Power BI |
| [Plausible](https://github.com/plausible/analytics) 🔁 | Google Analytics |
| [Umami](https://github.com/umami-software/umami) 🔁 | Google Analytics |
| [PostHog](https://github.com/PostHog/posthog) 🔁 | Mixpanel / Amplitude / Hotjar |
| [listmonk](https://github.com/knadh/listmonk) 🔁 | Mailchimp |
| [Medusa](https://github.com/medusajs/medusa) 🔁 | Shopify (headless commerce) |

## Developer Platforms

| Project | Replicates |
|---------|-----------|
| [Supabase](https://github.com/supabase/supabase) 🔁 | Firebase |
| [Appwrite](https://github.com/appwrite/appwrite) 🔁 | Firebase |
| [PocketBase](https://github.com/pocketbase/pocketbase) 🔁 | Firebase (single binary) |
| [Coolify](https://github.com/coollabsio/coolify) 🔁 | Heroku / Vercel / Netlify |
| [Dokploy](https://github.com/Dokploy/dokploy) 🔁 | Heroku / Vercel (open-core) |
| [Forgejo](https://codeberg.org/forgejo/forgejo) 🔁 | GitHub |
| [Hoppscotch](https://github.com/hoppscotch/hoppscotch) 🔁 | Postman |
| [Bruno](https://github.com/usebruno/bruno) 🔁 | Postman (offline, git-friendly) |
| [Activepieces](https://github.com/activepieces/activepieces) 🔁 | Zapier |
| [n8n](https://github.com/n8n-io/n8n) 🔁⚠️ | Zapier / Make (fair-code) |
| [SigNoz](https://github.com/SigNoz/signoz) 🔁 | Datadog / New Relic |
| [Uptime Kuma](https://github.com/louislam/uptime-kuma) 🔁 | Pingdom / StatusPage |

## AI Products

| Project | Replicates |
|---------|-----------|
| [Open WebUI](https://github.com/open-webui/open-webui) 🔁⚠️ | ChatGPT interface (custom licence requires keeping its branding) |
| [LibreChat](https://github.com/danny-avila/LibreChat) 🔁 | ChatGPT, multi-provider (acquired by ClickHouse, Nov 2025) |
| [LobeHub](https://github.com/lobehub/lobehub) 🔁⚠️ | ChatGPT, multi-provider (formerly LobeChat; derivative works need a commercial licence) |
| [AnythingLLM](https://github.com/Mintplex-Labs/anything-llm) 🔁 | ChatGPT + document Q&A |
| [Vane](https://github.com/ItzCrazyKns/Vane) 🔁 | Perplexity (formerly Perplexica) |
| [Ollama](https://github.com/ollama/ollama) 🔁 | Hosted model APIs, run locally |
| [Continue](https://github.com/continuedev/continue) 🔁 | GitHub Copilot |
| [Cline](https://github.com/cline/cline) 🔁 | Cursor agent mode |
| [OpenHands](https://github.com/OpenHands/OpenHands) 🔁 | Devin |
| [OpenWork](https://github.com/different-ai/openwork) 🔁🆕 | Claude Cowork / Codex desktop app (MIT core, open-core) |
| [ComfyUI](https://github.com/Comfy-Org/ComfyUI) 🔁 | Midjourney (node-based) |
| [InvokeAI](https://github.com/invoke-ai/InvokeAI) 🔁 | Midjourney / Firefly (now community-maintained) |

## Cybersecurity Tooling

| Project | Replicates |
|---------|-----------|
| [Ghidra](https://github.com/NationalSecurityAgency/ghidra) 🔁 | IDA Pro |
| [Cutter](https://github.com/rizinorg/cutter) 🔁 | IDA Pro / Binary Ninja |
| [ImHex](https://github.com/WerWolv/ImHex) 🔁 | 010 Editor |
| [ZAP](https://github.com/zaproxy/zaproxy) 🔁 | Burp Suite |
| [mitmproxy](https://github.com/mitmproxy/mitmproxy) 🔁 | Charles / Fiddler |
| [Nuclei](https://github.com/projectdiscovery/nuclei) 🔁 | Commercial vulnerability scanners |
| [OpenVAS](https://github.com/greenbone/openvas-scanner) 🔁 | Nessus |
| [Sliver](https://github.com/BishopFox/sliver) 🔁 | Cobalt Strike (authorised red-team use) |
| [Mythic](https://github.com/its-a-feature/Mythic) 🔁 | Cobalt Strike (authorised red-team use) |
| [Wazuh](https://github.com/wazuh/wazuh) 🔁 | Splunk ES / commercial XDR |
| [Security Onion](https://github.com/Security-Onion-Solutions/securityonion) 🔁⚠️ | Commercial NSM / SIEM (Elastic License 2.0) |
| [Velociraptor](https://github.com/Velocidex/velociraptor) 🔁 | Commercial EDR forensics |
| [MISP](https://github.com/MISP/MISP) 🔁 | Commercial threat-intel platforms |
| [Keycloak](https://github.com/keycloak/keycloak) 🔁 | Okta / Auth0 |
| [authentik](https://github.com/goauthentik/authentik) 🔁 | Okta / Auth0 |
| [NetBird](https://github.com/netbirdio/netbird) 🔁 | Tailscale / Zscaler Private Access |
| [Bitwarden](https://github.com/bitwarden/server) 🔁 | 1Password / LastPass |

## Watchlist: No Source or Unclear Licence Yet

Notable, but not yet meeting the bar for the main list. They'll move up once source and licence are public.

| Project | Replicates | Why it's here |
|---------|-----------|---------------|
| [reTS](https://github.com/DasSheep/reTS) | C&C Tiberian Sun / Red Alert 2 engine | Docs and devblog public; engine source not released. |
| [Reburn 3](https://github.com/reburndev/reburn3) | Burnout 3: Takedown | No licence file; last release 2023. |
| Astrocore (Luma's Workshop) | Super Mario Galaxy | Announced Sep 2026; not released. |
| [Mario Kart Wiicompiled](https://github.com/patchzyy/Wiicompiled) 🤖 | Mario Kart Wii | First Wii static recomp; licence unverified. |
| [Pilotwings 64: Recompiled](https://github.com/danielgomesvieira2000/pilotwings-64-recomp) | Pilotwings 64 | Licence unverified. |
| [Harvest Moon 64: Recompiled](https://github.com/HarvestMoon64Recomp/HarvestMoon64Recomp) | Harvest Moon 64 | Licence unverified. |
| [re:Blue](https://github.com/zolaware/reblue) | Blue Dragon (Xbox 360) | ReXGlue recomp; licence unverified. |
| [TiP-Recomp](https://github.com/SolarCookies/TiP-Recomp) | Viva Piñata: Trouble in Paradise | ReXGlue recomp; licence unverified. |

## Other Lists and Trackers

- [awesome-selfhosted](https://github.com/awesome-selfhosted/awesome-selfhosted): the big list of self-hostable software.
- [OSGameClones](https://github.com/opengaming/osgameclones): open-source clones and remakes of games.
- [awesome-game-remakes](https://github.com/radek-sprta/awesome-game-remakes): actively maintained game remakes.
- [OpenAlternative](https://openalternative.co): open-source alternatives to proprietary SaaS.
- [AlternativeTo (open source filter)](https://alternativeto.net/software/netflix/?license=opensource): crowd-sourced alternatives.

---

## Staying Safe: Fake Ports and Malware Bait

Popular releases attract impostor repositories, and in 2026 retro-gaming fans became a specific malware target ([Malwarebytes, Jun 2026](https://www.malwarebytes.com/blog/threat-intel/2026/06/retro-gaming-fans-are-the-new-target-for-fake-github-malware)). Patterns seen this year:

- **Copycat "PC port" repos** appeared within days of Dusk and Halo releasing. Typical signs:
  - SEO-stuffed READMEs ("pc port 60fps 4k windows 11 latest version 2026 download").
  - A few commits and no source tree, just a zip or a "download" link.
  - AI-generated banners and fake star or download badges.
  - Instructions to disable antivirus.
- **Stale or orphaned links:** some news coverage of the Halo port points to an older repository with no releases. Use [OpenCE's own Releases](https://github.com/OpenCommunityEdition/OpenCE) only.
- **Unofficial mirrors of viral projects:** third-party sites and forks hosting builds of the ArtCraft apps. The only official sources are github.com/storytold and getartcraft.com.
- **"Free Netflix Premium" and account-manager repos:** credential-stuffing tools or malware. Never run them.

Rule of thumb: get builds only from the official repo or site linked here, confirm the repo contains real source, and compare the org name with the team named in press coverage.

## Deliberately Excluded

- **Taken down:** re3 / reVC (GTA III and Vice City; DMCA and lawsuit), yuzu and its forks, the GoldenEye Native port, and Switch emulator repos removed in 2026 sweeps. Archived: MGB64 (GoldenEye, discontinued Aug 2026).
- **Derived from leaked source:** projects rewritten from leaked proprietary code, regardless of licence claims.
- **Piracy front-ends:** Netflix-style apps that stream from torrents or embed-scraper sites.
- **No licence:** projects without a licence file (e.g. some 2026 Xbox 360 recomps) until one is added.

## Legal Notes

- Nothing listed here distributes copyrighted game data, ROMs or proprietary assets. Where marked 📦, you must supply your own legally obtained copy.
- Reverse engineering for interoperability is treated differently by jurisdiction. Examples: DMCA §1201(f) in the US, the EU Software Directive Art. 6, and the *Copyright Act 1968* s 47D in Australia. This list is not legal advice.
- "Replica" means functional or behavioural equivalence. Trademarks belong to their owners and are used only to describe compatibility or inspiration.
- Projects that are taken down are removed rather than linked to mirrors.

## Contributing

Contributions are welcome. Read [CONTRIBUTING.md](CONTRIBUTING.md) first. The short version: link the official repo only, add one line on what it replicates, and make sure it is open source (or tagged ⚠️) and actually exists.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](LICENSE)

To the extent possible under law, the contributors have waived all copyright and related rights to this list.
