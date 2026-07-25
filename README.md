# GSonic Immersive — version manifest

`latest.json` publishes the current public release version of **GSonic Immersive**
so the application can tell you when a newer version is available.

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

This repository contains no application code — only the manifest above.

Updates are free for existing customers and are downloaded from your Gumroad
library, or via the download link in your original purchase email.
