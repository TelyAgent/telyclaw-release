# telyclaw-release

Public release storage for TelyClaw installers and update metadata.

## Current Release

- Version: `2.10.3`
- Date: `2026-04-30`
- macOS arm64 installer: `downloads/v2.10.3/TelyClaw-2.10.3-arm64.dmg`
- Download URL: https://media.githubusercontent.com/media/TelyAgent/telyclaw-release/main/downloads/v2.10.3/TelyClaw-2.10.3-arm64.dmg
- Update JSON: https://cdn.jsdelivr.net/gh/TelyAgent/telyclaw-release@main/updates/prod/update.json

## Layout

```text
updates/prod/update.json
updates/prod/update-manual.json
updates/test/update.json
updates/test/update-manual.json
downloads/v2.10.3/TelyClaw-2.10.3-arm64.dmg
```

Large installer files under `downloads/` are tracked with Git LFS.
