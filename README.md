# Resia theme for bb

This bb plugin adds the Resia palette:

- Light mode uses the cream "ash" colors of the Resia Portal.
- Dark mode uses charcoal surfaces and near-white text.
- Both modes use one rust accent, `#87401e`, for sent messages, buttons, and the selected thread row.
- Dark mode includes a matching code theme.

## Install

```bash
bb plugin install git:https://github.com/Bevoyhealth/bb-plugin-theme-resia --yes
```

Then select the theme in **Settings → Appearance**, or run:

```bash
bb theme set plugin:theme-resia:resia
```

## Edit

1. Clone this repository.
2. Install your clone with `bb plugin install path:<clone-dir> --yes`.
3. Edit `themes/resia.css`.
4. Reload the plugin with `bb plugin reload theme-resia`.

## Known limit

Three rules in `themes/resia.css` target bb markup directly, not theme tokens:

- the sent message bubble,
- the mention chips inside that bubble,
- the selected thread row.

A bb update can change that markup. If it does, those parts fall back to the token colors.
