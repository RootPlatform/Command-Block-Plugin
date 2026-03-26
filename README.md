# Command Block - Companion Plugin

The RootCompanion plugin connects your Minecraft server to Command Block, a Root app for managing and monitoring your Minecraft server from within your community.

**This plugin is only intended for use with the Command Block Root app.** It does not function as a standalone plugin.

## Compatibility

- Paper, Spigot, or Bukkit servers (1.16+)
- Java 17 or higher
- Not compatible with Vanilla, Forge, or Fabric servers

## Installation

1. Download the latest `RootCompanion.jar` from the [Releases](https://github.com/RootPlatform/Command-Block-Plugin/releases/latest) page

2. Upload `RootCompanion.jar` to your Minecraft server's `plugins/` folder

3. Restart your Minecraft server

4. After the server starts, the plugin generates a config file at `plugins/RootCompanion/config.yml` containing your API key and port

5. Open Command Block in your Root community, click **Add Server**, and choose **Manual Setup**

6. Enter your server's IP, the API key from `config.yml`, and the API port (default: 8080)

7. Click **Test Connection & Save** — your server will appear on the dashboard with real-time data

## What It Does

Once connected, the plugin streams real-time data to Command Block:

- Server status, TPS, and memory usage
- Player joins, leaves, and online player list
- In-game chat
- Server console output
- Player inventories (view and edit)
- World map (via Squaremap integration)

## Configuration

After first startup, the plugin creates `plugins/RootCompanion/config.yml`:

```yaml
api:
  key: rc_...      # Auto-generated API key (do not share)
  port: 8080       # HTTP/WebSocket server port
```

The API key authenticates the connection between your server and Command Block. If you regenerate it, you'll need to update the connection details in Command Block.

## Support

For issues or questions, reach out through your Root community or contact the Command Block team.
