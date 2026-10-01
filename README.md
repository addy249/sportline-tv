# Sportline TV

Sports IPTV player hosted on GitHub Pages. Select a channel and watch in the app. Includes search, retry, stop, and custom HTTPS HLS/MP4 playback.

## Channel source

11 selected public sports streams from https://github.com/iptv-org/iptv, using https://iptv-org.github.io/iptv/categories/sports.m3u. The bundled channels.json lets the app load even when the upstream playlist is unavailable. On each visit, the app attempts to refresh URLs for the selected channel IDs. It does not import the entire upstream list.

Channels include Red Bull TV, FUEL TV AU, Racer Network, ACC Digital Network, FloHockey, FloRacing, World of Freesports, 30A Golf Kingdom, FIFA+ United States, Strongman Champions League, and Racer Select.

These are community-submitted public stream links, not a guarantee of rights, availability, or a particular live match. Channels may carry replays, ads and scheduled programming. Geographic restrictions and stream failures can occur. No authentication, DRM, region or CORS bypass is provided. Browser playback requires HTTPS and provider CORS permission. No stream URLs entered by users are stored.

## Run and publish

Serve this directory with a static server, e.g. `python3 -m http.server 8080`.
GitHub Pages publishes the root of main. All asset paths are relative.

## Dependency

Vendored hls.js 1.6.13 (Apache-2.0), from https://cdn.jsdelivr.net/npm/hls.js@1.6.13/dist/hls.min.js. License: vendor/LICENSE-hls.txt.
