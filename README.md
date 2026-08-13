# gsonic-updates

Update manifests and installer downloads for GSonic applications. Installed
apps read a small per-app manifest here to learn when a newer version exists.
The check sends nothing — it is one read of a static file. This repository
contains no application code.

| App | Manifest |
|---|---|
| GSonic Evo 32 | `evo32.json` |
| GSonic Immersive | `immersive.json` |

Both manifests share one shape:

```json
{
  "latest_version": "1.0.0",
  "notes": "One plain ASCII line shown beside the notice.",
  "download_url": "https://github.com/ObsessiveCompulsiveAudiophile/gsonic-updates/releases/latest",
  "sha256": "optional - integrity of the attached installer",
  "size": 0
}
```

- `latest_version` — current public release, three numeric fields, compared
  against the running build.
- `download_url` — where the user's browser goes: the **direct installer
  link** for that version (auto-download; the releases page is the manual
  fallback).
- `sha256` / `size` — optional integrity facts for the attached installer.

Installers are attached to [Releases](https://github.com/ObsessiveCompulsiveAudiophile/gsonic-updates/releases).
An installer is inert without a license key — updates are free for existing
customers, activated with the key from the original purchase.

Manifest evolution is additive-only: fields are never renamed or removed —
installed applications parse these files forever.
