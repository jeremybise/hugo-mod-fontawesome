Work in progress...

FontAwesome available as a Hugo module.

Feather is a collection of simply beautiful open source icons. Each icon is designed on a 24x24 grid with an emphasis on simplicity, consistency, and flexibility. See https://github.com/FortAwesome/Font-Awesome.

## Use

Import the module into your Hugo project's site config:

```toml
[[module.imports]]
path = "github.com/jeremybise/hugo-mod-fontawesome"
```

The icons gets mounted in `assets/fontawesome`.

This means that they can be used like this in a Hugo template:

```html
{{ $icon := resources.Get "fontawesome/solid/search.svg" }} {{ $icon.Content |
safeHTML }}
```

Or, use the shortcode:

```html
{{ partial "fontawesome/icon" "solid/search" }}
```

See https://fontawesome.com/icons?d=gallery&m=free for a full list of icons.
