# Darcula Contrast for OpenIDEA

<img src="icon.svg" width="80" height="80" alt="Darcula Contrast logo">

JetBrains **Darcula Contrast** editor colors with the **Islands Darcula** interface for OpenIDEA 0.1.40+ (Plugin API 1.2+). PHP variables use the original **purple `#9876AA`**; function declarations and PHP function calls use **gold `#FFC66D`**.

## Colors

| Element | Color |
| --- | --- |
| Editor background | `#1E1F22` |
| Editor text | `#A9B7C6` |
| Current line | `#2B2D30` |
| Keywords | `#CC7832` |
| Strings | `#6A8759` |
| Numbers | `#6897BB` |
| Function declarations | `#FFC66D` |
| PHP variables | `#9876AA` |
| PHP function calls | `#FFC66D` |
| Fields and constants | `#9876AA` |
| Comments | `#808080` |

The editor scheme is generated from JetBrains' original `Darcula Contrast → Darcula` resources, including selections, search, diagnostics, diff, gutter, and terminal colors. The interface uses the original Islands Darcula resources. OpenIDEA supplies layout, spacing, and rounded corners; this plugin contains configuration only and needs no executable module or permissions.

JetBrains treats the [interface theme](https://www.jetbrains.com/help/phpstorm/user-interface-themes.html) and [editor color scheme](https://www.jetbrains.com/help/phpstorm/configuring-colors-and-fonts.html) separately. Darcula Contrast is an editor scheme, not the High Contrast interface theme. The inspected official PHP plugin supplies purple `#9876AA` for variables and parameters and inherits gold `#FFC66D` for function calls through its method attributes.

## Installation

1. Open **Settings → Plugins → ⚙ → Install Plugin from Package File…** and select this project's `plugin.toml`.
2. Alternatively, choose **Install Plugin from Disk…** and select the entire project folder.
3. In **Settings → Appearance → Theme**, select **Darcula Contrast**, then set the editor scheme to **Theme default**.

These local installation options are documented in [OpenIDEA's theme guide](https://github.com/l0ng-ai/openidea/blob/37c2a6048eea89d4f6db645622612358b643862b/docs/plugins/themes.md#building-packaging-installing). The upstream project's old Islands Darcula release does not contain these changes.

The plugin retains its original package ID, `longafter.islands-darcula`, for upgrade compatibility.

Before disabling or uninstalling the active theme, switch to the built-in **Islands Dark** theme to avoid the unavailable-theme message in OpenIDEA 0.1.40.

## Development

No dependencies or network access are needed to rebuild:

```sh
python3 scripts/generate.py
python3 scripts/validate.py
```

Edit the generator, then rebuild; `themes/darcula-contrast.*.json`, the token ledger, and provenance are generated files. Validation checks pinned hashes, reproducibility, manifest paths, supported tokens, aliases, source colors, and contrast thresholds.

## Sources and compatibility

Exact RGB values are preserved where the two editors expose equivalent roles. OpenIDEA's syntax categories and controls do not cover every PhpStorm attribute or font effect. Those mappings and inherited values are documented in [Color sources](docs/COLOR-SOURCES.md) and the generated [token ledger](docs/TOKEN-MAPPING.md). A side-by-side PhpStorm/OpenIDEA visual comparison has not been performed for this version.

This community port is licensed under Apache-2.0. Original colors are from JetBrains. See [third-party licenses](THIRD_PARTY_LICENSES.md) and [NOTICE](NOTICE).
