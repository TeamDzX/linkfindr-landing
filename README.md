# linkfindr-landing

LinkFindr marketing site, served into the Wix page via jsDelivr CDN (same
pattern as drawpad-landing).

**Embed in Wix (iframe):**

```html
<iframe
  src="https://cdn.jsdelivr.net/gh/TeamDzX/linkfindr-landing@main/index.html"
  style="width:100%; height:100%; border:0;"
  title="LinkFindr"></iframe>
```

Assets are referenced relatively, so everything resolves through the same CDN
path. Note jsDelivr caches `@main` for ~12h — after pushing changes, purge:
`https://purge.jsdelivr.net/gh/TeamDzX/linkfindr-landing@main/index.html`
