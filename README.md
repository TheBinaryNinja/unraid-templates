# Binary Ninja — Unraid Templates

Community Applications templates for the containers maintained by
[Binary Ninja](https://github.com/TheBinaryNinja) / [iFlip721](https://github.com/iFlip721).

Maintainer profile for Community Applications lives in [`ca_profile.xml`](ca_profile.xml).

## Templates

| App | Image | Project | Support |
| --- | --- | --- | --- |
| [AirConnect](AirConnect/airconnect.xml) | `iflip721/airconnect` | [iFlip721/AirConnect](https://github.com/iFlip721/AirConnect) | [Issues](https://github.com/iFlip721/AirConnect/issues) |
| [masqueradarr.aio](masqueradarr.aio/masqueradarr.aio.xml) | `iflip721/masqueradarr-aio` | [masqueradarr](https://thebinaryninja.github.io/masqueradarr/) | [Discord](https://discord.gg/baD3HGpkcD) |

**AirConnect** — AirPlay bridging to UPnP/Sonos and Chromecast devices, with a web UI for
diagnostics. Requires host networking; mDNS and SSDP discovery do not survive a bridge network.

**masqueradarr.aio** — self-hosted IPTV aggregator that pulls playlists and guide data from
multiple providers and serves them back as one unified, standards-compliant playlist + guide.

## Installing

These are published through Unraid **Community Applications** — search for the app name in
the *Apps* tab. To install a template directly instead, paste its raw URL into
*Docker → Add Container → Template*, e.g.

```
https://raw.githubusercontent.com/TheBinaryNinja/unraid-templates/main/AirConnect/airconnect.xml
```

## Contributing

Issues with a **template** (wrong path, missing variable, bad default) belong here. Issues with
the **application** itself belong on that project's own tracker, linked in the table above.

Templates follow the [Community Apps XML field reference](https://ca.unraid.net/submit/help/xml-field-reference).
Validate before opening a PR:

```sh
xmllint --noout ca_profile.xml */*.xml
```

## License

[MIT](LICENSE) — templates only. Each application carries its own license.
