# La Familia Fabric 1.21.1 Mods

Upload **Fabric 1.21.1 client mod JAR files** to `updates/files/mods/`.

GitHub Actions checks for `fabric.mod.json` and generates `updates/manifest.json` containing SHA-256 checksums. The launcher downloads only files named in this manifest.

Do **not** upload Forge 1.20.1 JAR files. Server-only Fabric mods should also not be shipped to client computers. Check each dependency and compatibility manually before publishing.

News remain in `news/news.json` and `news/images/`.
