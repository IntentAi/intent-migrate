# Server Structure Import

Two-step process: Export from Discord → Import to Intent

## Exporter (Discord Bot)

Runs on Discord, exports server structure as JSON.

**Captures:**
- Server metadata (name, icon, banner)
- All channels (categories, text, voice)
- All roles (hierarchy, permissions)
- Webhooks
- Emoji
- Channel settings

**Output:** `server-export.json`

## Importer (Intent CLI)

Reads JSON, recreates structure on Intent via API.

**Maps:**
- Channels → Channels (1:1)
- Roles → Roles (permission bitfield mapping)
- Webhooks → Webhooks (repointed to Intent)
- Emoji → Emoji (downloaded + reuploaded)

 Coming soon
