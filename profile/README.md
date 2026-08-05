<div align="center">

# CS2 Server Plugins

**Open-source plugins and gamemodes for Counter-Strike 2 dedicated servers**

Built on the [ModSharp](https://github.com/Kxnrl/modsharp-public) framework · C# / .NET

[![CS2](https://img.shields.io/badge/game-Counter--Strike%202-orange)](https://github.com/cs2-server-plugins)
[![Framework](https://img.shields.io/badge/framework-ModSharp-5865F2)](https://github.com/Kxnrl/modsharp-public)
[![Language](https://img.shields.io/badge/language-C%23-512BD4)](https://dotnet.microsoft.com/)

</div>

---

Every plugin here runs in production on public Counter-Strike 2 servers — these are not demos.
They cover complete gamemodes (Prop Hunt, TTT, Retakes, KZ, 1v1 Arenas), server administration,
and the infrastructure that sits underneath them.

## Gamemodes

| Plugin | What it does |
|---|---|
| [cs2-prophunt](https://github.com/cs2-server-plugins/cs2-prophunt) | Prop Hunt — core engine plus ranks, stats, shop and HUD modules |
| [cs2-ttt](https://github.com/cs2-server-plugins/cs2-ttt) | Trouble in Terrorist Town |
| [cs2-retakes](https://github.com/cs2-server-plugins/cs2-retakes) | Bomb-site retake practice with weapon allocation and zone-based spawns |
| [cs2-kreedz](https://github.com/cs2-server-plugins/cs2-kreedz) | KZ climbing — from-scratch, cs2kz-compatible |
| [cs2-arenas](https://github.com/cs2-server-plugins/cs2-arenas) | 1v1 / 2v2 arena dueling with queueing, loadouts and special rounds |
| [cs2-monster-mod](https://github.com/cs2-server-plugins/cs2-monster-mod) | AI monsters that navigate, chase and fight — HTN brain with A\* pathfinding |

## Server administration

| Plugin | What it does |
|---|---|
| [cs2-mapchooser](https://github.com/cs2-server-plugins/cs2-mapchooser) | End-of-map voting, RTV, nominations, map extensions |
| [cs2-vip](https://github.com/cs2-server-plugins/cs2-vip) | VIP framework — groups, perk registry, admin-panel integration |

## Progression & diagnostics

| Plugin | What it does |
|---|---|
| [cs2-progression](https://github.com/cs2-server-plugins/cs2-progression) | Missions, achievements and a season pass |
| [modsharp-profiler](https://github.com/cs2-server-plugins/modsharp-profiler) | EventPipe CPU profiler — captures traces and reports to Discord |

> More plugins are being migrated into this organisation. Browse the
> [full repository list](https://github.com/orgs/cs2-server-plugins/repositories) for everything published so far.

## Getting started

These are [ModSharp](https://github.com/Kxnrl/modsharp-public) modules. In general:

```bash
git clone https://github.com/cs2-server-plugins/<plugin>.git
cd <plugin>
dotnet build -c Release
# copy .build/modules/* into <server>/game/sharp/modules/
```

Each repository documents its own configuration, commands and dependencies — start with its README.

## Credits

Many of these are ports or reimplementations of existing SourceMod and CounterStrikeSharp plugins,
migrated to ModSharp. Original authors are credited in each repository's README, and upstream
licences are preserved. If something of yours is here and the attribution is wrong, open an issue —
it will be fixed.

Built on [ModSharp](https://github.com/Kxnrl/modsharp-public) by Kxnrl.

<div align="center">
<sub>Counter-Strike 2 · CS2 · dedicated server · plugins · gamemodes · ModSharp · C#</sub>
</div>
