### AntiAFK Plugin

#### Description
The AntiAFK plugin manages and mitigates player inactivity on Minecraft servers. Players idle for too long are marked AFK and may be kicked to ensure active player participation and server resource efficiency.

#### Features
- **Automatic AFK Detection:** Marks idle players as AFK after a configurable time.
- **Customizable Messages:** Personalize messages for AFK marking and kick notifications.
- **Title and Subtitle Notifications:** Displays prompts to AFK players via titles and subtitles.
- **Sound Alerts:** Customizable sounds for AFK marking and admin notifications.
- **Admin Notifications:** Alerts server operators of AFK players and kicks.
- **Permission Support:** Permissions for bypassing AFK checks and executing plugin commands.

#### Example Configuration
```yaml
# Configuration for the AntiAFK plugin
prefix: "&7[Antiafk]&r "

messages:
  afk: "&cYou are now AFK."
  notAfk: "&aYou are no longer AFK."
  kickReason: "&cKicked for inactivity."
  afkNotify: "&e{player} is now AFK."
  kickNotify: "&c{player} has been kicked for inactivity."

afk:
  afkCheckDelayTicks: 400 # Delay before considering a player as AFK (in ticks)
  kickDelayTicks: 200 # Delay before kicking an AFK player (in ticks)

sounds:
  afkSound: "ENTITY_PLAYER_LEVELUP"
  afkSoundVolume: 1.0
  afkSoundPitch: 1.0
  notifySound: "ENTITY_EXPERIENCE_ORB_PICKUP"
  notifySoundVolume: 1.0
  notifySoundPitch: 1.0

titles:
  afkTitle: '&cAFK'
  afkSubtitle: '&6Move to stay connected'
```

#### Commands
- `/antiafk reload`: Reloads the plugin configuration.
  - **Permission:** `antiafk.reload`

#### Permissions
- `antiafk.bypass`: Bypass AFK detection.
- `antiafk.reload`: Reload plugin configuration.

#### Installation
1. Download the plugin jar file.
2. Place the jar file in your server's plugins directory.
3. Restart your server to load the plugin.
4. Configure the plugin via `config.yml` in `plugins/AntiAFK`.
5. Use `/antiafk reload` to apply configuration changes without server restart.

#### Support
For issues or feature requests:
- Visit the [GitHub repository]([https://github.com/your/repository](https://github.com/Neast1337/AntiAFK)).
- Contact the plugin author on [SpigotMC]([https://www.spigotmc.org/members/author](https://www.spigotmc.org/members/neast.1408723/)).

---

Ownership Statement
This AntiAFK plugin is an original creation owned exclusively by Neast. All rights to the source code, configurations, and any other part of the plugin are reserved to Neast. No individual or entity is permitted to reproduce, copy, redistribute, or modify this plugin without the express permission of Neast.

Any infringement of this policy will be handled in accordance with applicable copyright laws.

For inquiries regarding the use of the plugin or to request specific permissions, please contact Neast via [Discord](https://discord.gg/jjEGrtt9t4).
