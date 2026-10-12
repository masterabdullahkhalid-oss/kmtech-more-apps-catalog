# KM Tech — More Apps Catalog

Har app ka **apna folder** — icon + details text. Easy for Khalid Mustafa Tech apps.

## Structure

```
apps/
  index.txt                 ← app folders ki list (order yahan se)
  video-to-mp3/
    details.txt             ← title, link, status, …
    icon.png                ← aap paste karo (512×512)
  image-to-pdf/
    details.txt
    icon.png
  _TEMPLATE_NEW_APP/        ← nayi app ke liye copy karo
```

## Nayi app add (3 steps)

1. `_TEMPLATE_NEW_APP` copy karke naya naam do (e.g. `my-cool-app`)
2. Us folder mein:
   - `icon.png` paste
   - `details.txt` edit (`title`, `packageName`, `playStoreUrl`, `status`)
3. `apps/index.txt` mein naye folder ka naam **ek line** pe add karo  
4. GitHub pe Upload / Commit

### `status` values
- `production` → Play pe published (Install / Open)
- `closed_testing` → Coming soon / closed testing section

## CDN (app uses this)

- Index: `https://cdn.jsdelivr.net/gh/masterabdullahkhalid-oss/kmtech-more-apps-catalog@main/apps/index.txt`
- Details: `.../apps/<folder>/details.txt`
- Icon: `.../apps/<folder>/icon.png`

Legacy single-file (optional backup): `more_apps_catalog.json`

## Local clone (easy editing)

```
git clone https://github.com/masterabdullahkhalid-oss/kmtech-more-apps-catalog.git
```

Desktop pe folder kholo → icons paste → `git add` → `git commit` → `git push`
