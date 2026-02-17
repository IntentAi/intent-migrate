# Intent Migration Toolkit

Tools for migrating Discord communities to [Intent](https://github.com/IntentAi/intent).

> Not yet implemented — scaffolding only.

## Components

| Tool | Purpose |
|------|---------|
| `server-import/exporter` | Discord bot that exports server structure |
| `server-import/importer` | CLI that imports structure into Intent |
| `bridge/` | Bidirectional message sync between Discord and Intent |
| `message-import/` | Historical message import (DiscordChatExporter format) |

## Migration Layers

1. **Server structure import** — channels, roles, permissions, settings
2. **Bridge bot** — real-time bidirectional sync during transition
3. **Message import** — optional historical message preservation

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md)

## License

MIT
