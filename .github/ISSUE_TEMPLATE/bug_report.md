---
name: 🐞 Bug report
about: Something does not work as it should, settings got lost, or the game crashes.
title: '[Bug] '
labels: ["bug"]
---
body:
  - type: markdown
    attributes:
      value: |
        Thanks for taking the time to report a bug!
        Please check the **[Troubleshooting](https://github.com/Rocket012/SyncSettings/wiki/Troubleshooting)** page first. Many problems are solved there.

        > **Lost settings?** Open *Options → SyncSettings → Backups / Undo* in-game. SyncSettings backs up `options.txt` before every change.

  - type: dropdown
    id: loader
    attributes:
      label: Mod loader
      options:
        - Fabric
        - NeoForge
        - Forge
    validations:
      required: true

  - type: input
    id: minecraft
    attributes:
      label: Minecraft version
      placeholder: e.g. 1.21.1
    validations:
      required: true

  - type: input
    id: mod-version
    attributes:
      label: SyncSettings file
      description: The exact file name of the SyncSettings jar in your mods folder.
      placeholder: e.g. syncsettings-fabric-1.2.0+1.21.1.jar
    validations:
      required: true

  - type: dropdown
    id: launcher
    attributes:
      label: Launcher
      options:
        - Modrinth App
        - CurseForge App
        - Prism Launcher
        - MultiMC
        - Official Minecraft Launcher
        - Other
    validations:
      required: true

  - type: dropdown
    id: instances
    attributes:
      label: Does the problem involve several instances or PCs?
      options:
        - "No, only one instance"
        - Several instances on one PC
        - Several PCs (cloud folder)
    validations:
      required: true

  - type: textarea
    id: what-happened
    attributes:
      label: What happened?
      description: What did you see, and what did you expect instead?
      placeholder: |
        I changed my mouse sensitivity in instance A, but instance B still uses the old value.
    validations:
      required: true

  - type: textarea
    id: steps
    attributes:
      label: Steps to reproduce
      placeholder: |
        1. Start instance A (Fabric 1.20.1) and change ...
        2. Close the game
        3. Start instance B (NeoForge 1.21.1)
        4. ...
    validations:
      required: true

  - type: textarea
    id: change-log
    attributes:
      label: SyncSettings log
      description: |
        Please paste the last lines of `syncsettings_changes.log`. It is in the folder `.syncsettings` in your user folder
        (Windows: `C:\Users\<you>\.syncsettings`), or in the folder shown at the bottom of the SyncSettings menu.
      render: text
    validations:
      required: true

  - type: textarea
    id: game-log
    attributes:
      label: Game log or crash report
      description: |
        If the game crashed or shows an error, upload `logs/latest.log` or the crash report from `crash-reports/`
        to [mclo.gs](https://mclo.gs) and paste the link here.
      placeholder: https://mclo.gs/...

  - type: textarea
    id: mods
    attributes:
      label: Other mods
      description: A list of your other mods, or the name of the modpack. Especially mods that change the options screen or settings.
      placeholder: e.g. Sodium, Iris, Mod Menu ... or "Fabulously Optimized 7.0"

  - type: textarea
    id: screenshots
    attributes:
      label: Screenshots
      description: Drag images in here if they help to show the problem.

  - type: checkboxes
    id: checks
    attributes:
      label: Checklist
      options:
        - label: I am using the newest SyncSettings version for my loader and Minecraft version.
          required: true
        - label: I searched the existing issues and this bug has not been reported yet.
          required: true
