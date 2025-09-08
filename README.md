# 🪄 SoulLock v1.2.1

**SoulLock** is a [Paper](https://papermc.io/) plugin for Minecraft 1.21.4 that lets you **bind tools and weapons to a specific player**.  
Once an item is Soul Bound, only the rightful owner can use, pick up, or retrieve it.  

This makes SoulLock ideal for **unique rewards, quest items, or server gear** where you don’t want trading or stealing.

---

## ✨ Features
- 🔒 **Soul Binding**: Lock any item to a player with a simple command.
- 📦 **Chest Storage**: Items can still be stored in chests, but only the owner can take them back out.
- 🚫 **Use Protection**: Non-owners can’t equip, attack, or interact with Soul Bound items.
- 🛡️ **Staff Bypass**: Toggle bypass mode for recovery/admin purposes.
- 💬 **Clean Messages**: Denial messages are throttled to avoid spam.
- ⚙️ **Fully Configurable**: Messages, lore text, and cooldowns can be customized in `config.yml`.
- 🔑 **Fine-grained Permissions**: Each command has its own permission node.

---

## ⚔️ Commands

| Command                  | Description                                 | Permission Node        |
|--------------------------|---------------------------------------------|------------------------|
| `/soullock help`         | 📖 Show available commands                   | `soullock.help`        |
| `/soullock` / `self`     | 🔒 Bind the held item to yourself            | `soullock.bind.self`   |
| `/soullock <player>`     | 🎁 Bind the held item to another player      | `soullock.bind.other`  |
| `/soullock info`         | 🔍 Show the owner of the held item           | `soullock.info`        |
| `/soullock clear`        | 🧹 Remove Soul Bound from the held item      | `soullock.clear`       |
| `/soullock bypass`       | 🛡️ Toggle staff bypass mode                  | `soullock.bypass`      |
| `/soullock reload`       | ♻️ Reload plugin config without restart      | `soullock.reload`      |

*(No permissions are granted by default. Assign them using a permissions plugin like [LuckPerms](https://luckperms.net/).)*

---

## 📦 Installation
1. Download the latest release from the [Releases](../../releases) page.  
2. Place the JAR into your server’s `plugins/` folder.  
3. Restart or reload your Paper server.  
4. Edit `plugins/Soullock/config.yml` if you want to customize messages/lore.  
5. Assign permission nodes using your permission manager (LuckPerms, etc).

---

## 🔧 Configuration
The plugin generates a `config.yml` on first run.  
- Change the lore text, message colors, and cooldowns.  
- Run `/soullock reload` in-game (with permission) to apply changes instantly.  

---

## 📜 Changelog
See the [CHANGELOG.md](CHANGELOG.md) for version history.  

---

## 📖 Wiki
For a full breakdown of usage, see the [Wiki](../../wiki).  
