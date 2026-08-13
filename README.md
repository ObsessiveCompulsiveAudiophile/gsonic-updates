# GSonic — version manifests

Small per-app manifests that let installed GSonic applications tell you when a
newer version is available. The check sends nothing — it is one read of a
static file. This repository contains no application code.

## GSonic Evo 32 — `evo32.json`

```json
{
  "latest_version": "1.0.0",
  "notes": "Current public release.",
  "download_url": "https://github.com/ObsessiveCompulsiveAudiophile/gsonic-updates/releases/download/v1.0.0/GSonicEvo32-1.0.0.msi",
  "sha256": "…",
  "size": 70000000
}
```

| Field | Meaning |
|---|---|
| `latest_version` | Current public release, compared against the running build |
| `notes` | Short, user-facing summary shown on the About page |
| `download_url` | The installer download for this version (attached to Releases here) |
| `sha256` / `size` | Integrity facts for the attached installer |

Installers are attached to [Releases](https://github.com/ObsessiveCompulsiveAudiophile/gsonic-updates/releases).
An installer is inert without a license key — updates are free for existing
customers, activated with the license key from the original purchase.

## GSonic Immersive — `latest.json`

```json
{
  "latest_version": "2.0.0",
  "notes": "Current public release.",
  "library_url": "https://app.gumroad.com/library"
}
```

| Field | Meaning |
|---|---|
| `latest_version` | Current public release, compared against the running build |
| `notes` | Short, user-facing summary shown alongside the notice |
| `library_url` | Where an existing customer downloads their free update |

Manifest shapes are additive-only: fields are never renamed or removed —
installed applications parse these files forever.
