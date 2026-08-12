# VComic OTA (standard)

Static OTA channel for VComic **standard** builds.

- `ota.json` — non-XR (phone/tablet) package metadata
- `ota-xr.json` — Android XR (`withXr`) package metadata
- `apks/` — per-ABI APKs for the **current** version (nonXr + withXr; old builds removed on publish)

Release notes i18n (optional keys on both manifests):

- `notes` — default **Simplified Chinese** (required for clients)
- `notes_zh_TW` — Traditional Chinese
- `notes_en_US` — English
- `notes_ja_JP` — Japanese
- `notes_ko_KR` — Korean
- `notes_ru_RU` — Russian

Do **not** mix standard and afdian APKs in the same repository.

Publish with:

```bash
python scripts/publish_ota.py --channel standard
# multi-language notes:
python scripts/publish_ota.py --channel standard --notes-i18n-file notes-i18n.json
```
