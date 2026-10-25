# MELK Studio OTA

OTA hosting for MELK Studio, using GitHub Pages.

## Publishing v1.1.0

1. Upload `ota/melk-1.1.0.zip` from the prepared GitHub Pages package.
2. Verify the uploaded ZIP is accessible via HTTPS and its SHA-256 is `06f49843e6aab0f64a3f83ebc2f393a2bea83e4b4566bf4f8edcd90966b7761c`.
3. Only then upload `ota/melk-version.json` from the same package.
4. Enable GitHub Pages from main / (root) in repository Settings → Pages.
5. Verify `https://muhammadusamataj.github.io/melk-studio-ota-/ota/melk-version.json` and the ZIP link.

**Migration note:** Previously installed APKs still use the Netlify endpoint. An APK built from the GitHub-OTA source (with matching signing certificate) or a working migration update is required to switch servers.

Never overwrite a published versioned ZIP; always publish a new version and checksum.
