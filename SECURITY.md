# Security policy

## Reporting a vulnerability

**Do not open a public issue.** These plugins run on live game servers, and a public report is a
working exploit for anyone reading it before a fix ships.

Use GitHub's private vulnerability reporting on the affected repository
(Security → Report a vulnerability), which reaches the maintainers without disclosure.

Useful in a report:
- which plugin and version
- what an attacker can do — crash the server, escalate to admin, read data
- reproduction steps, if you have them

## Scope

In scope: anything letting an unprivileged player crash a server, gain admin, or read data they
should not — including via chat commands, ConVars, or network messages a plugin handles.

Out of scope: vulnerabilities in Counter-Strike 2 itself or in the ModSharp framework. Report those
to Valve and to [ModSharp](https://github.com/Kxnrl/modsharp-public) respectively.
