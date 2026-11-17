# BlockForge Mods

Public catalog of Minecraft mods shared by the BlockForge community.

## Publishing a mod

1. Publish a GitHub Release in this repository and attach the `.jar` file.
2. Add a matching entry to `catalog.json` and commit it to `main`.
3. Refresh the catalog in BlockForge. Public listings and downloads do not require a BlockForge account.

Only publish files you created or have permission to redistribute. Never include Minecraft game files or credentials.

## Catalog format

```json
{
  "schemaVersion": 1,
  "mods": [
    {
      "slug": "example-mod",
      "name": "Example Mod",
      "description": "Short mod description",
      "version": "1.0.0",
      "gameVersions": ["1.21.4"],
      "loaders": ["Fabric"],
      "downloadUrl": "https://github.com/heka-dev/blockforge-mods/releases/download/v1.0.0/example-mod.jar",
      "sha256": "64-character-lowercase-sha256-hash"
    }
  ]
}
```

The `downloadUrl` must point to a `.jar` asset in this repository's Releases. `sha256` is the lowercase SHA-256 checksum of that file.
