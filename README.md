# OxyBoil Hugo Edition 

A slightly opinionated boilerplate for hugo new projects.

`v0.0.1-alpha`

[**Demo Preview Site**](https://oxyboil-hugo.vercel.app/)

---

Whenever I create a new hugo project with `hugo new site SITE_NAME` and `hugo new theme THEME_NAME` I have to spend time to edit and add files just so the new site can render without errors.
To avoid the hustle I created the **OxyBoil Hugo Edition**.

Feel free to use it if you like.

[Download the zip](https://github.com/Oxypteros/OxyBoil-hugo/archive/refs/heads/main.zip) and extract in your new site folder or press the ***Use this template*** button to use as repo template.

Nothing fancy.

## Changes from default new site

`config.toml`

* Add `theme = 'OxyBoil-theme'`

`archetypes/default.md`

* Draft set to false `draft: false`

`content/`

* Add content file for homepage `_index.md`
* Add test post files `test-1.md` and `test-2.md`

`themes/`

* Add boilerplate theme with `hugo new theme OxyBoil-theme`

## Changes from default new theme

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
