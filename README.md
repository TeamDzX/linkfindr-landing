# linkfindr-landing

LinkFindr marketing site. Served via **GitHub Pages** and embedded in the Wix
site as an iframe.

**Live URL:** https://teamdzx.github.io/linkfindr-landing/

**Embed in Wix (iframe / Embed a Site element):**

```html
<iframe
  src="https://teamdzx.github.io/linkfindr-landing/"
  style="width:100%; height:100%; border:0;"
  title="LinkFindr"></iframe>
```

Why Pages and not jsDelivr for the HTML: jsDelivr's /gh/ endpoint serves HTML
as `text/plain` + `nosniff`, so browsers refuse to render it. Pages serves
proper `text/html`, relative asset paths work, and pushes to `main` go live in
~a minute (no CDN purge dance). Individual images can still be hot-linked via
jsDelivr if ever needed elsewhere.

Assets live in `assets/` (web-sized JPEGs from real app screenshots +
ComfyUI-generated backdrop art). Page is fully self-contained: system fonts,
no external requests.
