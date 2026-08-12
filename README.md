# VComic OTA (standard)

Static OTA channel for VComic **standard** builds.

- `ota.json` — non-XR (phone/tablet) package metadata
- `ota-xr.json` — Android XR (`withXr`) package metadata
- `apks/` — per-ABI APKs for the **current** version (nonXr + withXr; old builds removed on publish)

Do **not** mix standard and afdian APKs in the same repository.

Publish with:

```bash
python scripts/publish_ota.py --channel standard
```
