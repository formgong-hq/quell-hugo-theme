# Quell

A one-page portfolio for an architect, a structural engineer or a small design studio. The demo studio, Mara Quell, its buildings, quotes and contacts are fictional.

![Quell](https://raw.githubusercontent.com/formgong/hugo-theme-quell/main/images/screenshot.png)

Demo: https://quell.formgong.com

## Install

As a Hugo module:

```sh
hugo mod init example.com/site
```

```toml
# hugo.toml
[module]
  [[module.imports]]
    path = "github.com/formgong-hq/hugo-theme-quell"
```

Or as a git submodule:

```sh
git submodule add https://github.com/formgong-hq/hugo-theme-quell.git themes/quell
echo 'theme = "quell"' >> hugo.toml
```

Every text of the page lives in `data/content.json`. Copy `exampleSite/data/content.json` into your site's `data/` folder and edit it there; without it the theme uses its own copy.

Hugo 0.156.0 or newer, no npm packages and no Hugo extended needed. Posts, tags, categories and the RSS feed use the theme's list and single layouts.

## Run the example site

```sh
cd exampleSite
hugo server --themesDir ../..
```

## Contact form

The contact form posts to Formgong (free plan): put your access key in `form.access_key` in `data/content.json`. To send it anywhere else, change `params.formAction` in `hugo.toml`.

## Fonts

Archivo: bundled as WOFF2 files (Latin and Latin Extended), no requests to Google Fonts. SIL Open Font License 1.1, the licence texts are next to the font files.

## License

MIT
