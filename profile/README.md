<div align="center">

# CS2 Server Plugins

**Open-source plugins and gamemodes for Counter-Strike 2 dedicated servers**

Built on the [ModSharp](https://github.com/Kxnrl/modsharp-public) framework · C# / .NET

[![CS2](https://img.shields.io/badge/game-Counter--Strike%202-orange)](https://github.com/cs2-server-plugins)
[![Framework](https://img.shields.io/badge/framework-ModSharp-5865F2)](https://github.com/Kxnrl/modsharp-public)
[![Language](https://img.shields.io/badge/language-C%23-512BD4)](https://dotnet.microsoft.com/)

</div>

---

Complete gamemodes, server administration and the infrastructure underneath them — all running in
production on public Counter-Strike 2 servers. These are not demos.

## Gamemodes

| Plugin | What it is |
|---|---|
| [cs2-prophunt](https://github.com/cs2-server-plugins/cs2-prophunt) | Prop Hunt — engine plus ranks, stats, shop and HUD modules |
| [cs2-ttt](https://github.com/cs2-server-plugins/cs2-ttt) | Trouble in Terrorist Town — roles, karma, shop, DNA scanner, body confirmation |
| [cs2-jailbreak](https://github.com/cs2-server-plugins/cs2-jailbreak) | Jailbreak — warden, last requests, special days, rebel tracking |
| [cs2-superpowers](https://github.com/cs2-server-plugins/cs2-superpowers) | 142 powers across 13 packs, plus a custom-rounds engine |
| [cs2-kreedz](https://github.com/cs2-server-plugins/cs2-kreedz) | KZ climbing — from-scratch, cs2kz-compatible |
| [cs2-mixscrims](https://github.com/cs2-server-plugins/cs2-mixscrims) | Mix and scrim matches — captains, team picking, leavers and substitutes |
| [cs2-retakes](https://github.com/cs2-server-plugins/cs2-retakes) | Bomb-site retake practice with weapon allocation and zone spawns |
| [cs2-furien](https://github.com/cs2-server-plugins/cs2-furien) | Asymmetric knife-vs-guns infection, in the Furien tradition |
| [cs2-arenas](https://github.com/cs2-server-plugins/cs2-arenas) | 1v1 / 2v2 arena dueling with queueing, loadouts, special rounds |
| [cs2-duels](https://github.com/cs2-server-plugins/cs2-duels) | 1v1 ladder with an in-game arena editor |
| [cs2-invisiblemod](https://github.com/cs2-server-plugins/cs2-invisiblemod) | Hide-and-seek — frozen invisible hiders, sound-hunting seekers |
| [cs2-minihumans](https://github.com/cs2-server-plugins/cs2-minihumans) | Shrinks players into mini-humans, with custom camera and collision |
| [cs2-1vsall](https://github.com/cs2-server-plugins/cs2-1vsall) | One versus all |

## Event & round modes

| Plugin | What it is |
|---|---|
| [cs2-event-manager](https://github.com/cs2-server-plugins/cs2-event-manager) | Deploy every event mode to one server and switch between them live |
| [cs2-fun-rounds](https://github.com/cs2-server-plugins/cs2-fun-rounds) | Config-driven engine for fun and special rounds |

## Server administration

| Plugin | What it is |
|---|---|
| [cs2-mapchooser](https://github.com/cs2-server-plugins/cs2-mapchooser) | End-of-map voting, RTV, nominations, map extensions |
| [cs2-vip](https://github.com/cs2-server-plugins/cs2-vip) | VIP framework — groups, perk registry, admin-panel integration |
| [cs2-calladmin](https://github.com/cs2-server-plugins/cs2-calladmin) | In-game report system — players report cheaters, admins claim and resolve |
| [cs2-afk-manager](https://github.com/cs2-server-plugins/cs2-afk-manager) | Moves idle players to spectator or kicks them after configurable thresholds |
| [cs2-hitmark](https://github.com/cs2-server-plugins/cs2-hitmark) | Attacker-only hitmarkers, damage numbers and hitsounds |
| [cs2-reset-score](https://github.com/cs2-server-plugins/cs2-reset-score) | Players reset their own scoreboard stats; admins can set anyone's |
| [cs2-round-end-sounds](https://github.com/cs2-server-plugins/cs2-round-end-sounds) | Weighted-random song at round end, per-client volume and prefs |
| [cs2-skill-autobalance](https://github.com/cs2-server-plugins/cs2-skill-autobalance) | Skill-based round-end team balancer — CTPS with outlier detection |

## Progression & diagnostics

| Plugin | What it is |
|---|---|
| [cs2-progression](https://github.com/cs2-server-plugins/cs2-progression) | Missions, achievements and a season pass |
| [modsharp-profiler](https://github.com/cs2-server-plugins/modsharp-profiler) | EventPipe CPU profiler — captures traces, reports to Discord |

## Getting started

These are [ModSharp](https://github.com/Kxnrl/modsharp-public) modules:

```bash
git clone https://github.com/cs2-server-plugins/<plugin>.git
cd <plugin>
dotnet build -c Release
# copy .build/modules/* into <server>/game/sharp/modules/
```

Each repository documents its own commands, configuration and dependencies — start with its README.
Configuration files ship as `.example`; copy and edit rather than editing in place, so a redeploy
does not overwrite your settings.

## Contributing

Issue templates, a pull-request template and the contribution guide apply across every repository
here — see [CONTRIBUTING](https://github.com/cs2-server-plugins/.github/blob/main/CONTRIBUTING.md).

Security issues go through private reporting, never a public issue:
[SECURITY](https://github.com/cs2-server-plugins/.github/blob/main/SECURITY.md). These plugins run on
live game servers, so a public report is a working exploit for anyone who reads it first.

## Credits

Many of these are ports or reimplementations of existing SourceMod and CounterStrikeSharp plugins,
migrated to ModSharp. Original authors are credited in each repository, and upstream licences are
preserved — several of these are GPL or AGPL precisely because the work they descend from is.

If something of yours is here and the attribution is wrong, open an issue and it will be fixed.

Built on [ModSharp](https://github.com/Kxnrl/modsharp-public) by Kxnrl.

<div align="center">
<sub>Counter-Strike 2 · CS2 · dedicated server · plugins · gamemodes · ModSharp · Source 2 · C#</sub>
</div>
