# 📜 Changelog — SoulLock

All notable changes to **SoulLock** will be documented in this file.  
Format follows [Keep a Changelog](https://keepachangelog.com/en/1.0.0/) and versions use [Semantic Versioning](https://semver.org/).

---

## [1.2.1] — 2025-09-08
### Changed
- `/soullock help` is now **dynamic**:
  - Only shows commands the player actually has permission for.
  - Removed permission node text from help output to keep it player-friendly.
- Internal refactoring:
  - Consolidated messages into `config.yml` (shorter code, easier maintenance).
  - Reduced redundant event/message handling while preserving all functionality.

### Fixed
- Bug with `OWNER_NAME_KEY` access in `getOwnerName` (PersistentDataType was missing).  

---

## [1.2.0] — 2025-09-06
### Added
- **New permissions & commands**:
  - `/soullock bypass` → `soullock.bypass`
  - `/soullock info` → `soullock.info`
  - `/soullock clear` → `soullock.clear`
  - `/soullock <player>` → `soullock.bind.other`
  - `/soullock self` → `soullock.bind.self`
  - `/soullock reload` → `soullock.reload`
  - `/soullock help` → `soullock.help`
- **Config.yml support**:
  - Customize all plugin messages, colors, and lore text.
  - Adjust throttle delay for chat spam protection.
  - Hot-reload with `/soullock reload`.
- **Permission-controlled help**: every command requires explicit permission; no defaults.

### Changed
- All user-facing text changed from **“Soul Locked”** → **“Soul Bound”**.
- Chest interactions updated: non-owners can store Soul Bound items but **cannot remove them**.

---

## [1.0.0] — Initial Release
- Basic soul binding of items to a player’s UUID.
- Lore line `"Soul Locked to %player%"`.
- Prevented other players from using, equipping, or picking up locked items.
- Allowed storage in chests but no restrictions on retrieval.
