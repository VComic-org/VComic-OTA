# VComic OTA (standard)

Static OTA channel for VComic **standard** builds.

- `ota.json` — current version metadata (clients poll this file)
- `apks/` — per-ABI release APKs

Do **not** mix standard and afdian APKs in the same repository.

Publish with:

```bash
python scripts/publish_ota.py --channel standard
```
