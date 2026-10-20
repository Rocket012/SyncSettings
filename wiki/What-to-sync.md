# What to sync

Under **What to sync…** you choose which settings belong to a profile. Anything you leave out stays local to each instance.

SyncSettings can read and write:

- `options.txt` (video, sound, controls, key bindings, …)
- Mod configs in `config/*.json` and `config/*.toml`

## Migrations between Minecraft versions

Some options were renamed or changed between Minecraft versions. SyncSettings uses version-aware migration rules to translate them. If a value cannot be applied safely, SyncSettings keeps the existing value and writes the reason to `syncsettings_changes.log`.
