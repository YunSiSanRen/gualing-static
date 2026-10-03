# gualing-static

Static assets (obfuscated JavaScript, CSS and webfonts) for the gualing.top frontend,
served to browsers through a CDN.

This repository contains **build artifacts only** — no sources, no configuration, no credentials.

## Layout

    js/          obfuscated application bundles
    js/libs/     third-party libraries vendored for offline fallback
    fonts/       webfonts (woff2)
    images/      page icons and background patterns
    data/        static JSON data loaded at runtime

Stylesheets are **not** kept here: the pages load `css/*.css` from their own origin.

## Versioning

Every CI/CD publish is tagged (`vX.Y.Z`). Pages reference a pinned tag, e.g.

    https://cdn.jsdmirror.com/gh/YunSiSanRen/gualing-static@v1.0.0/js/utils.js
