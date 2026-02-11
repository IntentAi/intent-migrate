# Intent Migration Toolkit

Tools for migrating from Discord to Intent.

## Why Migration Matters

Communities won't move without:
1. Their server structure (channels, roles, permissions)
2. Their bots
3. A transition period where both platforms work

This toolkit makes migration frictionless.

## Components

### 1. Server Structure Import
Export Discord server structure → Import to Intent

**What gets migrated:**
- Server name, icon, banner
- Categories and channels (text, voice)
- Roles with permission mappings
- Webhooks
- Emoji
- Channel settings (topics, slowmode, NSFW)

### 2. Bridge Bot
Run both platforms simultaneously during transition.

**Features:**
- Bidirectional message sync
- Edit/delete propagation
- Attachment forwarding
- User avatar masquerading
- Gradual migration support

### 3. Message Import (Optional)
Import historical messages from Discord.

Uses DiscordChatExporter JSON format.

## Structure

```
intent-migrate/
├── server-import/
│  ├── exporter/   # Discord bot (exports structure)
│  └── importer/   # Intent CLI (imports structure)
├── bridge/      # Bidirectional sync bot
└── message-import/  # Historical message import
```

## Usage

In development: Setup and usage guides

## Migration Strategy

### Layer 1: Webhook Compatibility (Easiest Win)
Change webhook URL → existing integrations work

### Layer 2: Server Structure Import (Removes Objection)
Export → Import in 5 minutes

### Layer 3: Bridge Bot (Enables Gradual Migration)
Run both platforms, sync in real-time

### Layer 4: Message Import (Optional)
Preserve history if needed

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md)

## License

MIT License - See [LICENSE](LICENSE)
