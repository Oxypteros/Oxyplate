# OxyBoil Hugo Edition (v0.0.1-alpha)

An opinionated boilerplate of hugo new site/theme.
[Demo Preview Site](https://oxyboil-hugo.vercel.app/)

## Changes from hugo new site

`config.toml`

* Change `baseURL`
* Add `theme = 'OxyBoil-theme'`

`archetypes/default.md`

* Draft set to false `draft: false`

`content/`

* Add content file for homepage `_index.md`
* Add test post files `test-1.md` and `test-2.md`

`themes/`

* Add boilerplate theme with `hugo new theme OxyBoil-theme`

## Changes from hugo new theme

* Add `FILE IDENTIFIER` to `404.html`
* Add `{{ define "main" }} FILE IDENTIFIER {{- end }}` to `index.html`
* Add `assets/css/styles.css` file
* Add `i18n/en.toml` file, and months translations in `en.toml`

`theme.toml`

* Change minimum version `min_version = "0.108.0"`

`_default/`

* Add `_markup/` folder and files `render-link.html` (with `target="blank"`), `render-image.html` (for `hugo version > 0.108.0`)
* Add `lang="{{ .Site.Language.Lang }}"` to `<html>` tag of `baseof.html`
* Add `{{ define "main" }} FILE IDENTIFIER {{- end }}` to `list.html` and `single.html`

`partials/`

* Add `FILE IDENTIFIER` to `footer.html`, `head.html` and `header.html`