# Awesome Open Replicas [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of open-source reimplementations, reverse-engineered engines, decompilations and faithful replicas of commercial software, games, SaaS products and platforms.

Every few weeks someone ships an open-source version of something that used to be locked up: a 20-year-old console game running natively on PC, a clean-room engine for a classic RTS, a self-hosted stand-in for a SaaS tool you pay per seat for. This list tracks the ones that are real, maintained, and legitimately distributed.

**Legend**

| Tag | Meaning |
|-----|---------|
| 🔬 | Reverse-engineered or clean-room **reimplementation** (behaviour/protocol/engine recreated from the original) |
| 🧬 | **Decompilation** or static **recompilation** of an original binary, often with a native port |
| 🔁 | Functional open-source **replica / alternative** to a commercial product |
| 🆕 | Released or hit a major milestone in **2026** |
| 📦 | Bring your own copy — you must supply legally owned original game data or assets |

---

## Contents

- [Games: Native Ports from Decompilations](#games-native-ports-from-decompilations)
- [Games: Reimplemented Engines](#games-reimplemented-engines)
- [Games: Recompilation Toolchains and Trackers](#games-recompilation-toolchains-and-trackers)
- [Emulators](#emulators)
- [Operating Systems and Compatibility Layers](#operating-systems-and-compatibility-layers)
- [Protocol and Server Reimplementations](#protocol-and-server-reimplementations)
- [Office and Productivity](#office-and-productivity)
- [Adobe and Creative Suite](#adobe-and-creative-suite)
- [Streaming and Media (Netflix, Spotify, YouTube)](#streaming-and-media-netflix-spotify-youtube)
- [Communication (Slack, Discord, Zoom)](#communication-slack-discord-zoom)
- [Social Platforms](#social-platforms)
- [Business SaaS](#business-saas)
- [Developer Platforms](#developer-platforms)
- [AI Products](#ai-products)
- [Cybersecurity Tooling](#cybersecurity-tooling)
- [Other Lists and Trackers](#other-lists-and-trackers)
- [Staying Safe: Fake Ports and Malware Bait](#staying-safe-fake-ports-and-malware-bait)
- [Legal Notes](#legal-notes)
- [Contributing](#contributing)

---

## Games: Native Ports from Decompilations

All of these require you to provide your own original game files. 📦

| Project | Replicates | Notes |
|---------|-----------|-------|
| [Dusk / Dusklight](https://github.com/TwilitRealm/dusk) 🧬🆕📦 | The Legend of Zelda: Twilight Princess (GameCube) | Native port built on the completed TP decompilation, released May 2026. MIT. Windows, macOS, Linux, Android, iOS, Steam Deck. Renamed Dusklight in 1.2. |
| [zeldaret/tp](https://github.com/zeldaret/tp) 🧬 | Twilight Princess | The matching decompilation that Dusk is built on. |
| [Ship of Harkinian](https://github.com/HarbourMasters/Shipwright) 🧬📦 | The Legend of Zelda: Ocarina of Time | The Harbour Masters port that kicked off the modern decomp-port wave. |
| [2 Ship 2 Harkinian](https://github.com/HarbourMasters/2ship2harkinian) 🧬📦 | Zelda: Majora's Mask | Harbour Masters' MM port. |
| [Starship](https://github.com/HarbourMasters/Starship) 🧬📦 | Star Fox 64 | Native port from the SF64 decomp. |
| [SpaghettiKart](https://github.com/HarbourMasters/SpaghettiKart) 🧬📦 | Mario Kart 64 | Harbour Masters port with custom track support. |
| [sm64coopdx](https://github.com/coop-deluxe/sm64coopdx) 🧬📦 | Super Mario 64 | Online co-op PC port based on the SM64 decomp. |
| [n64decomp/sm64](https://github.com/n64decomp/sm64) 🧬 | Super Mario 64 | The original matching decomp behind most SM64 ports. |
| [Perfect Dark port](https://github.com/fgsfdsfgs/perfect_dark) 🧬📦 | Perfect Dark (N64) | Native PC port of the Perfect Dark decomp. |
| [MGB64](https://github.com/akratch/mgb64) 🧬🆕📦 | 1997 N64 first-person shooter | Decompilation + native PC/macOS port, started mid-2026. Experimental. |
| [Zelda64Recomp](https://github.com/Zelda64Recomp/Zelda64Recomp) 🧬📦 | Majora's Mask | Static recompilation (not a full decomp) with mods, high frame rates and widescreen. |
| [UnleashedRecomp](https://github.com/hedge-dev/UnleashedRecomp) 🧬📦 | Sonic Unleashed (Xbox 360) | Static recompilation to native PC. |
| [RSDKv5 Decompilation](https://github.com/RSDKModding/RSDKv5-Decompilation) 🧬📦 | Sonic Mania's engine (Retro Engine v5) | Decompiled engine for Sonic Mania and related titles. |
| [OpenGOAL](https://github.com/open-goal/jak-project) 🧬📦 | Jak and Daxter series (PS2) | Recreates Naughty Dog's GOAL language/compiler to run the games natively. |

## Games: Reimplemented Engines

Engine rewrites that read the original data files. 📦 unless stated.

| Project | Replicates | Notes |
|---------|-----------|-------|
| [reTS](https://github.com/DasSheep/reTS) 🔬🆕 | C&C Tiberian Sun / Red Alert 2 / Yuri's Revenge engine | Clean-room, oracle-tested reimplementation. Docs and devblog public; engine source not yet released. |
| [Reburn 3](https://github.com/reburndev/reburn3) 🔬📦 | Burnout 3: Takedown | WIP reimplementation; currently runs via Cxbx-Reloaded. |
| [OpenCaptive](https://github.com/yeager/OpenCaptive) 🔬🆕📦 | Captive (1990) and Liberation: Captive 2 (1993) | C/SDL3 reimplementation with extensive disassembly docs. |
| [OpenRA](https://github.com/OpenRA/OpenRA) 🔬 | Command & Conquer, Red Alert, Dune 2000 | Modernised RTS engine. |
| [Vanilla Conquer](https://github.com/TheAssemblyArmada/Vanilla-Conquer) 🔬📦 | C&C Tiberian Dawn / Red Alert | Portable builds of the EA-released source. |
| [OpenSAGE](https://github.com/OpenSAGE/OpenSAGE) 🔬📦 | EA SAGE engine (C&C Generals, BFME) | Engine reimplementation. |
| [OpenMW](https://openmw.org) 🔬📦 | The Elder Scrolls III: Morrowind | Mature, moddable engine replacement. |
| [Daggerfall Unity](https://github.com/Interkarma/daggerfall-unity) 🔬📦 | The Elder Scrolls II: Daggerfall | Full recreation in Unity. |
| [OpenTTD](https://github.com/OpenTTD/OpenTTD) 🔬 | Transport Tycoon Deluxe | Ships with free replacement assets; no original data required. |
| [OpenRCT2](https://github.com/OpenRCT2/OpenRCT2) 🔬📦 | RollerCoaster Tycoon 2 | Reverse-engineered, now far beyond the original. |
| [OpenLoco](https://github.com/OpenLoco/OpenLoco) 🔬📦 | Chris Sawyer's Locomotion | Same approach as OpenRCT2. |
| [CorsixTH](https://github.com/CorsixTH/CorsixTH) 🔬📦 | Theme Hospital | Engine reimplementation. |
| [DevilutionX](https://github.com/diasurgical/devilutionX) 🔬📦 | Diablo / Hellfire | Based on a reconstructed Diablo source. |
| [fheroes2](https://github.com/ihhub/fheroes2) 🔬📦 | Heroes of Might and Magic II | Engine recreation. |
| [VCMI](https://github.com/vcmi/vcmi) 🔬📦 | Heroes of Might and Magic III | Engine rewrite with mod support. |
| [OpenEnroth](https://github.com/OpenEnroth/OpenEnroth) 🔬📦 | Might and Magic VI–VIII | Engine reimplementation. |
| [Julius](https://github.com/bvschaik/julius) / [Augustus](https://github.com/Keriew/augustus) 🔬📦 | Caesar III | Faithful engine (Julius) and enhanced fork (Augustus). |
| [OpenXcom](https://github.com/OpenXcom/OpenXcom) 🔬📦 | UFO: Enemy Unknown / X-COM: Terror from the Deep | Clone of the original engine. |
| [Arx Libertatis](https://github.com/arx/ArxLibertatis) 🔬📦 | Arx Fatalis | Cross-platform port of the released source. |
| [OpenClaw](https://github.com/pjasicek/OpenClaw) 🔬📦 | Captain Claw (1997) | Engine reimplementation. |
| [OpenLara](https://github.com/XProger/OpenLara) 🔬📦 | Tomb Raider (1996) | Classic TR engine; also runs on very low-end hardware. |
| [ScummVM](https://github.com/scummvm/scummvm) 🔬📦 | LucasArts, Sierra and hundreds of adventure games | Reimplements dozens of engines. |
| [OpenJK](https://github.com/JACoders/OpenJK) 🔬📦 | Jedi Academy / Jedi Outcast | Community-maintained engine. |
| [ioquake3](https://github.com/ioquake/ioq3) 🔬📦 | Quake III Arena | The long-running Q3 source port. |

## Games: Recompilation Toolchains and Trackers

| Project | What it does |
|---------|--------------|
| [N64Recomp](https://github.com/N64Recomp/N64Recomp) | Static recompiler that turns N64 binaries into C, the basis for most "Recomp" ports. |
| [XenonRecomp](https://github.com/hedge-dev/XenonRecomp) | Static recompiler for Xbox 360 PowerPC executables. |
| [decomp.dev](https://decomp.dev) | Progress tracker for many decompilation projects. |
| [Read Only Memo: decomp list](https://readonlymemo.com/decompilation-projects-and-n64-recompiled-list) | Regularly updated list of decomps, recomps and finished ports. |

## Emulators

Emulators recreate hardware rather than software, but they are the oldest form of open replica.

| Project | Replicates |
|---------|-----------|
| [Dolphin](https://github.com/dolphin-emu/dolphin) 🔬 | GameCube / Wii |
| [PCSX2](https://github.com/PCSX2/pcsx2) 🔬 | PlayStation 2 |
| [RPCS3](https://github.com/RPCS3/rpcs3) 🔬 | PlayStation 3 |
| [shadPS4](https://github.com/shadps4-emu/shadPS4) 🔬 | PlayStation 4 |
| [xemu](https://github.com/xemu-project/xemu) 🔬 | Original Xbox |
| [Xenia](https://github.com/xenia-project/xenia) 🔬 | Xbox 360 |
| [Cemu](https://github.com/cemu-project/Cemu) 🔬 | Wii U |
| [ares](https://github.com/ares-emulator/ares) 🔬 | Multi-system, accuracy-focused |
| [MAME](https://github.com/mamedev/mame) 🔬 | Arcade and thousands of other machines |

## Operating Systems and Compatibility Layers

| Project | Replicates |
|---------|-----------|
| [ReactOS](https://github.com/reactos/reactos) 🔬 | Windows NT (binary-compatible OS) |
| [Wine](https://gitlab.winehq.org/wine/wine) 🔬 | Win32 API on Linux/macOS |
| [Proton](https://github.com/ValveSoftware/Proton) 🔬 | Wine + DXVK stack for Windows games on Linux |
| [Darling](https://github.com/darlinghq/darling) 🔬 | macOS userland on Linux |
| [Haiku](https://github.com/haiku/haiku) 🔬 | BeOS |
| [AROS](https://github.com/aros-development-team/AROS) 🔬 | AmigaOS 3.1 API |
| [Asahi Linux](https://asahilinux.org) 🔬 | Reverse-engineered drivers for Apple Silicon Macs |

## Protocol and Server Reimplementations

Open servers or clients built by reverse-engineering a proprietary protocol.

| Project | Replicates |
|---------|-----------|
| [Headscale](https://github.com/juanfont/headscale) 🔬 | Tailscale's coordination server |
| [Vaultwarden](https://github.com/dani-garcia/vaultwarden) 🔬 | Bitwarden server API (lightweight Rust rewrite) |
| [Samba](https://github.com/samba-team/samba) 🔬 | Windows SMB file sharing and Active Directory |
| [librespot](https://github.com/librespot-org/librespot) 🔬 | Spotify Connect client (Premium account required) |
| [TrinityCore](https://github.com/TrinityCore/TrinityCore) 🔬 | World of Warcraft server (for private development and research) |

## Office and Productivity

| Project | Replicates |
|---------|-----------|
| [LibreOffice](https://github.com/LibreOffice/core) 🔁 | Microsoft Office |
| [ONLYOFFICE Docs](https://github.com/ONLYOFFICE/DocumentServer) 🔁 | Microsoft 365 / Google Docs (high OOXML fidelity) |
| [Collabora Online](https://github.com/CollaboraOnline/online) 🔁 | Office for the web |
| [CryptPad](https://github.com/cryptpad/cryptpad) 🔁 | Google Docs, end-to-end encrypted |
| [AppFlowy](https://github.com/AppFlowy-IO/AppFlowy) 🔁 | Notion |
| [AFFiNE](https://github.com/toeverything/AFFiNE) 🔁 | Notion + Miro |
| [Anytype](https://github.com/anyproto/anytype-ts) 🔁 | Notion, local-first |
| [Outline](https://github.com/outline/outline) 🔁 | Confluence / Notion wiki |
| [Docmost](https://github.com/docmost/docmost) 🔁 | Confluence |
| [Joplin](https://github.com/laurent22/joplin) 🔁 | Evernote |
| [Logseq](https://github.com/logseq/logseq) 🔁 | Roam Research |
| [Excalidraw](https://github.com/excalidraw/excalidraw) 🔁 | Whiteboard tools |
| [Stirling-PDF](https://github.com/Stirling-Tools/Stirling-PDF) 🔁 | Adobe Acrobat (PDF toolkit) |
| [Nextcloud](https://github.com/nextcloud/server) 🔁 | Dropbox / Google Drive / Microsoft 365 |
| [Immich](https://github.com/immich-app/immich) 🔁 | Google Photos / iCloud Photos |
| [Cal.com](https://github.com/calcom/cal.com) 🔁 | Calendly |
| [Documenso](https://github.com/documenso/documenso) 🔁 | DocuSign |

## Adobe and Creative Suite

| Project | Replicates |
|---------|-----------|
| [GIMP](https://gitlab.gnome.org/GNOME/gimp) 🔁 | Photoshop |
| [Krita](https://invent.kde.org/graphics/krita) 🔁 | Photoshop (painting) / Clip Studio |
| [Graphite](https://github.com/GraphiteEditor/Graphite) 🔁 | Photoshop + Illustrator, node-based (Apache 2.0) |
| [Inkscape](https://gitlab.com/inkscape/inkscape) 🔁 | Illustrator |
| [Penpot](https://github.com/penpot/penpot) 🔁 | Figma / Adobe XD |
| [Scribus](https://github.com/scribusproject/scribus) 🔁 | InDesign |
| [darktable](https://github.com/darktable-org/darktable) 🔁 | Lightroom |
| [RawTherapee](https://github.com/Beep6581/RawTherapee) 🔁 | Camera Raw / Lightroom |
| [Kdenlive](https://invent.kde.org/multimedia/kdenlive) 🔁 | Premiere Pro |
| [Shotcut](https://github.com/mltframework/shotcut) 🔁 | Premiere Pro |
| [Olive](https://github.com/olive-editor/olive) 🔁 | Premiere Pro (node-based, in development) |
| [Natron](https://github.com/NatronGitHub/Natron) 🔁 | After Effects / Nuke compositing |
| [Synfig](https://github.com/synfig/synfig) 🔁 | Adobe Animate |
| [Blender](https://projects.blender.org/blender/blender) 🔁 | Maya / Cinema 4D / After Effects 3D |
| [Audacity](https://github.com/audacity/audacity) 🔁 | Audition |
| [Ardour](https://github.com/Ardour/ardour) 🔁 | Pro Tools / Audition multitrack |
| [OBS Studio](https://github.com/obsproject/obs-studio) 🔁 | Commercial streaming / screen capture |

> Photopea and Affinity are free but **not** open source, so they are not listed.

## Streaming and Media (Netflix, Spotify, YouTube)

| Project | Replicates |
|---------|-----------|
| [Jellyfin](https://github.com/jellyfin/jellyfin) 🔁 | Netflix-style experience for your own library (and Plex/Emby) |
| [Kodi](https://github.com/xbmc/xbmc) 🔁 | Media centre / smart TV UI |
| [MediaCMS](https://github.com/mediacms-io/mediacms) 🔁 | Video hosting CMS |
| [PeerTube](https://github.com/Chocobozzz/PeerTube) 🔁 | YouTube (federated) |
| [Owncast](https://github.com/owncast/owncast) 🔁 | Twitch (self-hosted live streaming) |
| [Navidrome](https://github.com/navidrome/navidrome) 🔁 | Spotify for your own music |
| [Audiobookshelf](https://github.com/advplyr/audiobookshelf) 🔁 | Audible |
| [Clone-Wars](https://github.com/GorvGoyl/Clone-Wars) 🔁 | 100+ UI clones of Netflix, Spotify, YouTube, Airbnb and more (learning projects) |

> Front-end "Netflix clones" are mostly portfolio projects using the TMDB API. They replicate the UI, not the streaming platform. Anything that pulls in content you don't have rights to is excluded from this list.

## Communication (Slack, Discord, Zoom)

| Project | Replicates |
|---------|-----------|
| [Mattermost](https://github.com/mattermost/mattermost) 🔁 | Slack |
| [Rocket.Chat](https://github.com/RocketChat/Rocket.Chat) 🔁 | Slack |
| [Zulip](https://github.com/zulip/zulip) 🔁 | Slack (threaded) |
| [Stoat (formerly Revolt)](https://stoat.chat) 🔁 | Discord. Renamed in October 2025 after a trademark notice. |
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
| [Planka](https://github.com/plankanban/planka) 🔁 | Trello |
| [WeKan](https://github.com/wekan/wekan) 🔁 | Trello |
| [Twenty](https://github.com/twentyhq/twenty) 🔁 | Salesforce / HubSpot CRM |
| [Odoo Community](https://github.com/odoo/odoo) 🔁 | NetSuite / SAP Business One |
| [ERPNext](https://github.com/frappe/erpnext) 🔁 | NetSuite / SAP |
| [NocoDB](https://github.com/nocodb/nocodb) 🔁 | Airtable |
| [Baserow](https://github.com/bram2w/baserow) 🔁 | Airtable |
| [Teable](https://github.com/teableio/teable) 🔁 | Airtable |
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
| [Dokploy](https://github.com/Dokploy/dokploy) 🔁 | Heroku / Vercel |
| [Forgejo](https://codeberg.org/forgejo/forgejo) 🔁 | GitHub |
| [Hoppscotch](https://github.com/hoppscotch/hoppscotch) 🔁 | Postman |
| [Bruno](https://github.com/usebruno/bruno) 🔁 | Postman (offline, git-friendly) |
| [Activepieces](https://github.com/activepieces/activepieces) 🔁 | Zapier |
| [n8n](https://github.com/n8n-io/n8n) 🔁 | Zapier / Make (fair-code licence, not OSI open source) |
| [SigNoz](https://github.com/SigNoz/signoz) 🔁 | Datadog / New Relic |
| [Uptime Kuma](https://github.com/louislam/uptime-kuma) 🔁 | Pingdom / StatusPage |

## AI Products

| Project | Replicates |
|---------|-----------|
| [Open WebUI](https://github.com/open-webui/open-webui) 🔁 | ChatGPT interface (check its licence's branding terms before rebranding) |
| [LibreChat](https://github.com/danny-avila/LibreChat) 🔁 | ChatGPT, multi-provider |
| [LobeChat](https://github.com/lobehub/lobe-chat) 🔁 | ChatGPT, multi-provider |
| [AnythingLLM](https://github.com/Mintplex-Labs/anything-llm) 🔁 | ChatGPT + document Q&A |
| [Perplexica](https://github.com/ItzCrazyKns/Perplexica) 🔁 | Perplexity |
| [Ollama](https://github.com/ollama/ollama) 🔁 | Hosted model APIs, run locally |
| [Continue](https://github.com/continuedev/continue) 🔁 | GitHub Copilot |
| [Cline](https://github.com/cline/cline) 🔁 | Cursor agent mode |
| [OpenHands](https://github.com/All-Hands-AI/OpenHands) 🔁 | Devin |
| [ComfyUI](https://github.com/comfyanonymous/ComfyUI) 🔁 | Midjourney (node-based) |
| [InvokeAI](https://github.com/invoke-ai/InvokeAI) 🔁 | Midjourney / Firefly |

## Cybersecurity Tooling

| Project | Replicates |
|---------|-----------|
| [Ghidra](https://github.com/NationalSecurityAgency/ghidra) 🔁 | IDA Pro |
| [Cutter](https://github.com/rizinorg/cutter) 🔁 | IDA Pro / Binary Ninja |
| [ImHex](https://github.com/WerWolv/ImHex) 🔁 | 010 Editor |
| [ZAP](https://github.com/zaproxy/zaproxy) 🔁 | Burp Suite |
| [Nuclei](https://github.com/projectdiscovery/nuclei) 🔁 | Commercial vulnerability scanners |
| [OpenVAS](https://github.com/greenbone/openvas-scanner) 🔁 | Nessus |
| [Sliver](https://github.com/BishopFox/sliver) 🔁 | Cobalt Strike (authorised red-team use) |
| [Mythic](https://github.com/its-a-feature/Mythic) 🔁 | Cobalt Strike (authorised red-team use) |
| [Wazuh](https://github.com/wazuh/wazuh) 🔁 | Splunk ES / commercial XDR |
| [Security Onion](https://github.com/Security-Onion-Solutions/securityonion) 🔁 | Commercial NSM / SIEM |
| [Velociraptor](https://github.com/Velocidex/velociraptor) 🔁 | Commercial EDR forensics |
| [MISP](https://github.com/MISP/MISP) 🔁 | Commercial threat-intel platforms |
| [Keycloak](https://github.com/keycloak/keycloak) 🔁 | Okta / Auth0 |
| [authentik](https://github.com/goauthentik/authentik) 🔁 | Okta / Auth0 |
| [NetBird](https://github.com/netbirdio/netbird) 🔁 | Tailscale / Zscaler Private Access |
| [Bitwarden](https://github.com/bitwarden/server) 🔁 | 1Password / LastPass |

## Other Lists and Trackers

- [awesome-selfhosted](https://github.com/awesome-selfhosted/awesome-selfhosted) — the big list of self-hostable software.
- [OSGameClones](https://github.com/opengaming/osgameclones) — open-source clones and remakes of games.
- [awesome-game-remakes](https://github.com/radek-sprta/awesome-game-remakes) — actively maintained game remakes.
- [OpenAlternative](https://openalternative.co) — open-source alternatives to proprietary SaaS.
- [AlternativeTo (open source filter)](https://alternativeto.net/software/netflix/?license=opensource) — crowd-sourced alternatives.

---

## Staying Safe: Fake Ports and Malware Bait

Popular releases attract impostor repositories. When Dusk landed in 2026, copycat "PC port" repos appeared within days. Common warning signs:

- README is stuffed with search keywords ("pc port 60fps 4k windows 11 latest version 2026 download").
- The repo has a handful of commits and **no source code**, only a release archive or a "download" link.
- AI-generated banner images and fake star/download badges.
- Instructions to disable your antivirus or run an unsigned `.exe` from a zip.
- Org name doesn't match the team credited by press coverage or the project's own website.

Always get builds from the official repo or website linked in this list, and check that the repo actually contains the source tree.

## Legal Notes

- Nothing listed here distributes copyrighted game data, ROMs, or proprietary assets. Where marked 📦, you must supply your own legally obtained copy.
- Reverse engineering for interoperability is treated differently by jurisdiction (e.g. DMCA §1201(f) in the US, EU Software Directive Art. 6, the *Copyright Act 1968* s 47D in Australia). This list is not legal advice.
- "Replica" here means functional or behavioural equivalence. Trademarks belong to their owners and are used only to describe what each project is compatible with or inspired by.
- Projects that were taken down (e.g. by DMCA) are removed rather than linked to mirrors.

## Contributing

Contributions welcome. Read [CONTRIBUTING.md](CONTRIBUTING.md) first; the short version is: official repo link only, one line on what it replicates, and it must be open source and actually exist.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](LICENSE)

To the extent possible under law, the contributors have waived all copyright and related rights to this list.
