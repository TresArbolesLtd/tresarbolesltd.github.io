# Tres Arboles website

Plain static HTML and CSS. No build step, no dependencies.

## Layout

| Path | Purpose |
| --- | --- |
| `index.html` | Home: company intro, app list, contact |
| `support/` | Support URL for the App Store and Google Play |
| `privacy/`, `terms/` | Index pages linking to each app's documents |
| `<app-slug>/` | One folder per app: about page, `privacy/`, `terms/` |
| `assets/` | `site.css` and logo files |
| `404.html` | Not-found page |

## Preview locally

```
node dev-server.js
```

Then open http://localhost:4173.

## Add a new app

1. Copy `pure-intervals/` to a new folder named for the app and edit the three pages.
2. Add the app to the list in `index.html` and `support/index.html`.
3. Add its documents to `privacy/index.html` and `terms/index.html`.

## Store listing URLs (per app)

- Support URL: `/support/`
- Privacy Policy URL: `/<app-slug>/privacy/`
- Marketing URL (optional): `/<app-slug>/`
