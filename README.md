# SyncSettings  
**Minecraft settings & profile synchronization (Multi-Loader)**

SyncSettings helps you keep your Minecraft settings consistent across **instances**, **servers**, and **Minecraft versions** using **profiles** and **snapshots** — with safe migrations and change logging.

This repository is the **public issue tracker & documentation hub** for SyncSettings.  
> The source code is intentionally **not public**.

---

## Downloads

- Modrinth: `LINK_HERE`
- CurseForge: `LINK_HERE`

---

## What SyncSettings does

- **Profiles:** Save and reuse named profiles for your settings  
- **Snapshots:** Read/write common settings and config formats (e.g. `options.txt`, `config/*.json`, `config/*.toml`)
- **Migrations:** Includes version-aware migration rules to handle major option changes
- **Conflict handling:** Safe fallback + a clear change log (`syncsettings_changes.log`)
- **Multi-loader support:** Designed for modern loaders (Fabric / Forge / NeoForge) plus legacy support depending on release

---

## Quick start

1. Install the correct loader for your Minecraft version (**Fabric / Forge / NeoForge**).
2. Drop the SyncSettings `.jar` into your `mods` folder.
3. Launch Minecraft once.
4. Create a profile and save a snapshot.
5. Switch instance/version and load the same profile again.

---

## Reporting bugs / requesting features (Issues)

Issues are welcome — please include as much detail as possible.

### Before you open an issue
- Make sure you’re using the **latest version** of SyncSettings for your Minecraft version/loader.
- Check if a similar issue already exists.

### Include this info
- Minecraft version:
- Loader (Fabric / Forge / NeoForge) + loader version:
- SyncSettings version:
- Singleplayer or server:
- Log files:
  - `latest.log` (or server log)
  - `syncsettings_changes.log` (if relevant)
- Steps to reproduce:
- Expected result vs actual result:

### What to upload
- Please **do not** upload private tokens, accounts, or personal data.
- If configs contain sensitive info, redact them.

---

## Modpack permissions

**Modpacks are allowed** to include SyncSettings **as an unmodified `.jar`**.

**Conditions:**
- **No reuploads / no mirrors:** Do not rehost the `.jar` on other sites.
- **Use official sources:** Prefer downloading via the official Modrinth/CurseForge project pages.
- **No modified distributions:** Forks/ports/modified builds may not be distributed without explicit permission.

If you need special permissions (mirrors, forks, ports), open an issue or contact me.

---

## License

**All Rights Reserved (Closed Source)**  
This repository contains documentation and issue tracking only. The source code is not publicly available.

---

## FAQ

### Is the mod open source?
No. SyncSettings is **closed source**.

### Can I use this in my modpack?
Yes — modpacks are allowed under the conditions above.

### Where are configuration files stored?
Profiles are stored outside instances, typically under:
- `~/.syncsettings/profiles`

(Exact paths may vary by OS / launcher.)

---

## Contact

- GitHub Issues: Use this repository
