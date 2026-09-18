# Unraid templates — SEC844

Unraid Community Applications templates maintained by SEC844.

| Application | Template | Project |
|---|---|---|
| Analysarr | [`templates/analysarr.xml`](templates/analysarr.xml) | [SEC844/Analysarr](https://github.com/SEC844/Analysarr) |

## Analysarr

A self-hosted dashboard that brings together Emby or Jellyfin, Sonarr, Radarr and your torrent client
(qBittorrent, Deluge or Transmission), and shows, for every movie and series, what is actually wrong
across the stack: duplicates left behind by an upgrade, orphan torrents seeding a file nothing links to
anymore, broken hardlinks, content seeded on a single tracker, and episodes Sonarr downloaded but the
media server never imported. Cleanup, hardlink repair and deletions always show a preview first.

Install it from Community Applications, or add the container manually with this template URL:

```
https://raw.githubusercontent.com/SEC844/unraid-templates/main/templates/analysarr.xml
```

**Mounts matter**: map your data share with the same host path and the same container path as in your
media server, torrent client, Sonarr and Radarr, otherwise hardlinks cannot be detected. Settings →
Paths → Path diagnostics reports a missing mount immediately.

## Support

[Unraid forum support thread](https://forums.unraid.net/topic/200625-support-sec844-analysarr/), or [issues on the project repository](https://github.com/SEC844/Analysarr/issues).

## License

[AGPL-3.0](LICENSE), same as Analysarr itself.
