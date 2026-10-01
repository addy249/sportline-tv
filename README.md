# Sportline TV

A responsive static sports streaming hub for GitHub Pages. Three official provider destinations, plus an in-browser HLS/MP4 player for user-supplied authorized HTTPS streams. No accounts, backend, telemetry or stored stream URLs.

## Run

Serve this directory using any static server, e.g. `python3 -m http.server 8080`. Open http://localhost:8080.

## Hosting

Publish the repository root from the `main` branch through Settings → Pages → Deploy from a branch. All asset paths are relative, so project Pages URLs work.

## Coverage

Provider links are not a live EPG and do not assert an event is currently on air. Official services open in a separate tab. Account requirements and regional rights apply. No third-party streams are republished or proxied. The custom player needs a browser-compatible stream and the provider's CORS permission; it cannot bypass authentication, DRM or geography restrictions.

Sources checked October 1, 2026:
- https://www.redbull.tv/en
- https://www.dazn.com/en-GB/help/articles/36029102113053-fifa-on-dazn-everything-you-need-to-know
- https://support.olympics.com/hc/en-gb/articles/1500009814861-What-is-Olympic-Channel

## Dependency

Vendored hls.js 1.6.13 (Apache-2.0), downloaded from https://cdn.jsdelivr.net/npm/hls.js@1.6.13/dist/hls.min.js. See vendor/LICENSE-hls.txt.
