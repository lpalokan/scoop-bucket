# lpalokan scoop-bucket

A [Scoop](https://scoop.sh) bucket for [BMad Manager](https://github.com/lpalokan/bmad-manager).

## Install

```
scoop bucket add lpalokan https://github.com/lpalokan/scoop-bucket
scoop install bmad-manager
```

## Update

```
scoop update bmad-manager
```

User data lives in `%LOCALAPPDATA%\bmad-manager` and Windows Credential Manager
(outside the install dir), so it is preserved across updates.

## Maintenance

The `version`, `url`, and `hash` in `bucket/bmad-manager.json` are updated
automatically by the `release` workflow in the
[bmad-manager](https://github.com/lpalokan/bmad-manager) repo on each published
release. Manual edits are normally unnecessary.

> Note: the manifest is seeded with placeholder `version`/`hash` values and
> becomes installable once the first release carrying a
> `bmad-manager-windows-x64-portable.zip` asset is published.
