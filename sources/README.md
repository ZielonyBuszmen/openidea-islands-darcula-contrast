# Pinned color sources

These files support development, provenance, and offline rebuilds. The installed plugin does not download or read them.

- `jetbrains/`: unmodified public IntelliJ Community color resources pinned to `idea/262.10968.63`. The Darcula Contrast overlay inherits the base Darcula scheme; the three UI resources form the Islands Darcula parent chain.
- `openidea-token-groups.json`: official `themeTokenGroups(tokens.css)` output; Islands Dark values record host fallbacks only.
- `openidea-mapping.json`: the original three mapping tables exported from the official `intellijTheme.ts` converter.
- `UPSTREAM.json`: pinned commits, paths, public links, SHA-256 hashes, and the read-only official PHP plugin inspection record. The PHP plugin archive and its proprietary resources are not bundled.
- `token-provenance.json`: generated per-token source, mapping status, customizations, approximations, and host fallbacks.

See the root LICENSE, NOTICE, and THIRD_PARTY_LICENSES.md for attribution. Do not commit personal `.icls` files, private projects in screenshots, account details, or local user settings.
