# Contributing

Thanks for taking the time. These are plugins for Counter-Strike 2 dedicated servers, built on the
[ModSharp](https://github.com/Kxnrl/modsharp-public) framework.

## Reporting a bug

Open an issue on the repository it affects and fill in the template. The version fields matter more
than they look — a plugin bug and a framework bug present identically from the outside, and the
server log usually distinguishes them immediately.

**Redact credentials** from configs and logs before pasting: database passwords, Discord webhook
URLs, API keys.

## Pull requests

- Build before opening: `dotnet build -c Release`
- Match the surrounding code — these repos share conventions, and consistency matters more than
  personal preference
- Say how you tested it. Server-side behaviour frequently differs from what compiles
- Keep a PR to one concern

## Porting from other frameworks

Many of these are ports of SourceMod or CounterStrikeSharp plugins. If you port something:

- **Credit the original** in the README, with a link
- **Preserve the upstream licence.** A derivative of GPL code stays GPL — that is not optional
- Note what you deliberately changed rather than implying a 1:1 port

## Security

Do not open a public issue for a vulnerability. See [SECURITY.md](SECURITY.md).
