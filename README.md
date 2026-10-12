# KM Tech — More Apps Catalog

Remote catalog for **More Apps by Khalid Mustafa Tech** (used by KM Status Saver and sibling Play apps).

## Edit apps

1. Open [`more_apps_catalog.json`](more_apps_catalog.json)
2. Add / edit / change `status`:
   - `production` — published on Play (Install / Open)
   - `closed_testing` — closed testing / coming soon section
3. Commit on `main`

Apps refresh in the client via CDN (no Play Store app update required for list changes).

## Fields

| Field | Required | Notes |
|-------|----------|--------|
| `title` | yes | App name |
| `description` | yes | Short line |
| `packageName` | yes | Play package id |
| `playStoreUrl` | yes | Store listing HTTPS URL |
| `iconKey` | yes | Local drawable name in the Android apps (e.g. `catalog_arrow_game`) |
| `iconUrl` | no | Optional remote image URL (future) |
| `status` | yes | `production` or `closed_testing` |
| `featured` | no | Highlight badge |
| `enabled` | no | Default `true`; set `false` to hide without deleting |

## CDN URL (app uses this)

```
https://cdn.jsdelivr.net/gh/masterabdullahkhalid-oss/kmtech-more-apps-catalog@main/more_apps_catalog.json
```

Raw GitHub fallback:

```
https://raw.githubusercontent.com/masterabdullahkhalid-oss/kmtech-more-apps-catalog/main/more_apps_catalog.json
```
