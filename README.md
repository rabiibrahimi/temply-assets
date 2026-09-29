# temply-assets

Public, static assets used by emails built with Temply Builder. Email clients (Gmail, Outlook, etc.) must be able to fetch these images anonymously, so this repo is public. It contains images only, no code.

Served via jsDelivr, pinned to a tag:

```
https://cdn.jsdelivr.net/gh/rabiibrahimi/temply-assets@v1/play/circle-dark.png
```

Tags are never moved. Changes get a new tag, so emails that were already sent keep loading the same files.

## Play buttons (`play/`)

PNG at 2x (192px tall) for retina; editable SVG sources are in `play/svg/`.

| Shape | Variants |
|---|---|
| `circle` | `circle-dark`, `circle-light`, `circle-red` |
| `rounded` | `rounded-dark`, `rounded-light`, `rounded-red` |
| `pill` | `pill-dark`, `pill-light`, `pill-red` |

`dark` = translucent black with white ring, `light` = white with dark triangle, `red` = red with white triangle.
