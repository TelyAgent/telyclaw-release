# telyclaw-release

Public release storage for TelyClaw installers and update metadata.

## Current Release

- Version: `2.10.3`
- Date: `2026-04-30`
- macOS arm64 installer: `downloads/v2.10.3/TelyClaw-2.10.3-arm64.dmg`
- Download URL: https://media.githubusercontent.com/media/TelyAgent/telyclaw-release/main/downloads/v2.10.3/TelyClaw-2.10.3-arm64.dmg
- Update JSON: https://cdn.jsdelivr.net/gh/TelyAgent/telyclaw-release@main/updates/prod/update.json
- MAS Update JSON: https://cdn.jsdelivr.net/gh/TelyAgent/telyclaw-release@main/updates/prod/mas-update.json

## Layout

```text
updates/prod/update.json
updates/prod/update-manual.json
updates/prod/mas-update.json
downloads/v2.10.3/TelyClaw-2.10.3-arm64.dmg
```

Large installer files under `downloads/` are tracked with Git LFS.

## Update Channels

Only the production update channel is used. Test update manifests are not part of the client update flow.

- `updates/prod/latest.json` is reserved for Tauri updater manifests used by direct-distribution builds. It must include Tauri updater signatures and updater artifacts such as `.app.tar.gz`, not plain DMG files.
- `updates/prod/mas-update.json` is used by Mac App Store builds only for version prompts. The App Store URL lives in this JSON so the client package does not hardcode an App Store ID before listing.
- `updates/prod/update.json` and `updates/prod/update-manual.json` remain available for manual download metadata and compatibility.
