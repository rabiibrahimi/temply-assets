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

## Release rules

1. **Never move or delete a tag.** Every email already sent points at a tag (`@v1`) forever.
2. Changing or replacing an existing file? Commit it, then push a **new** tag (`v2`, `v3`…) and point new emails at it.
3. Only *adding* new files still needs a new tag before they're used, because jsDelivr serves from the tag, not from `main`.
4. Never rename or remove files in a way that affects older tags. Old tags stay as they are.
