# SentinelCore lists

Public distribution of **signed** tracker-list updates for the SentinelCore Android app.

This repository contains data files only:

- `manifest.json` — signed manifest (`sentinel-lists/1`)
- `manifest.json.sig` — detached Ed25519 signature (64 raw bytes)
- list files such as `sentinel-default.txt` (GPL-3.0-or-later)

The app downloads the `lists-latest` release over HTTPS and verifies the signature with a public key compiled into the app **before** parsing or activating any list.

There is no application source code here. The signing private key is **not** stored in this repository.

Default fetch URL: <https://github.com/SuperfastSimon/SentinelCore-lists/releases/download/lists-latest/manifest.json>
