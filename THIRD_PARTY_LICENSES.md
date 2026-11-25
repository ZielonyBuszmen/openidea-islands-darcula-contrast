# Third-party licenses and modification notice

Original mappings, scripts, documentation, and ported theme configurations use Apache License 2.0. See [LICENSE](LICENSE) for the full license and [NOTICE](NOTICE) for attribution. Vendored reference files remain unmodified.

| Upstream | Pinned version | Material and purpose | License |
| --- | --- | --- | --- |
| JetBrains / intellij-community | `idea/262.10968.63` / `8062c061ff33e22041d9f1844db5b8b8a6b5e4d7` | Original UI and editor color resources in `sources/jetbrains/`, including the Darcula Contrast overlay; authoritative palette | Apache-2.0 source resources; JetBrains NOTICE retained |
| l0ng-ai / openidea | `v0.1.40` / `37c2a6048eea89d4f6db645622612358b643862b` | Official example structure, token inventory, and converter mappings extracted as JSON | Apache-2.0 |

Original JetBrains attribution:

```text
This software includes code from IntelliJ IDEA
Copyright (C) JetBrains s.r.o.
https://www.jetbrains.com/idea/
```

NOTICE retains this attribution and identifies the reused color resources. JetBrains' root `LICENSE.txt` for the pinned version contains Open-Source Build Terms that describe Apache-2.0 licensing for open-source software; the original text is retained in [licenses/JetBrains-OPEN-SOURCE-BUILD-TERMS.txt](licenses/JetBrains-OPEN-SOURCE-BUILD-TERMS.txt). This plugin does not distribute an IDEA application build.

**Modification notice:** `themes/darcula-contrast.*.json` are generated, modified ports with file-header attribution. JetBrains UI keys and inherited Darcula Contrast editor attributes are mapped to OpenIDEA CSS tokens, with documented role approximations and derived expressions. PHP variables and function calls use the original colors verified in the official PHP plugin and platform fallback attributes. These files are not official JetBrains exports.

The official proprietary JetBrains PHP plugin, version `252.28539.167`, was inspected read-only to verify its variable colors. Only factual color observations and source hashes are recorded in `sources/UPSTREAM.json`; its archive, XML, and executable code are not bundled or relicensed here.

JetBrains logos, fonts, icons, JARs, and proprietary executable code are not copied or distributed. Product names describe compatibility and original sources. No independent NOTICE was found for the other referenced third-party projects; no additional copyright years or permissions are asserted.
