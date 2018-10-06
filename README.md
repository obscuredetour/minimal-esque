# Minimal-esque
#### A dark minimal-esque theme for Hugo

Personal blog theme powered by [Hugo](https://gohugo.io) using the [Minimal](https://github.com/calintat/minimal) theme as a boilerplate.
A live demo is should hopefully be available soon.
<!-- A live demo is available [here](https://themes.gohugo.io/theme/minimal/). -->

## Changes
Here are the most notable changes
* Removal of Bootstrap, jQuery and all their dependencies. Yet still fully responsive.
* Article card layout built using Flexbox only
* Navigation mechanics built using only vanilla JavaScript


## Installation

You can install the theme either as a clone or submodule.

I recommend the latter. From the root of your Hugo site, type the following:

```
$ git submodule add https://github.com/obscuredetour/minimal.git themes/minimal-esque
$ git submodule init
$ git submodule update
```

Now you can get updates to Minimal-esque in the future by updating the submodule:

```
$ git submodule update --remote themes/minimal-esque
```

## Configuration

After installation, take a look at the `exampleSite` folder inside `themes/minimal-esque`.

To get started, copy the `config.toml` file inside `exampleSite` to the root of your Hugo site:

```
$ cp themes/minimal-esque/exampleSite/config.toml .
```

Now edit this file and add your own information. Note that some fields can be omitted.

I recommend you use the theme's archetypes so now delete your site's `archetypes/default.md`.

Customization options might be revisted in the future.

<!--## Features

You can tweak the look of the theme to suit your needs in a number of ways:

 - The accent colours can be changed by using the `accent` field in `config.toml`.

- You can also change the background colour by using `backgroundColor`.

For best results, I recommend you use a dark accent colour with a light background, for example:

```sass
[params]
    accent = "red"
    showBorder = true
    backgroundColor = "white"
```

### Fonts

The theme uses [Google Fonts](https://fonts.google.com) to load its font. To change the font:

```toml
[params]
    font = "Raleway" # should match the name on Google Fonts!
``` -->

### Syntax highlighting

The theme supports syntax highlighting thanks to [highlight.js](https://highlightjs.org).

It's disabled by default, so you have to enable it by setting `highlight` to `true` in your config.

You can change the style used for the highlighting by using the `highlightStyle` field.

Only the "common" languages will be loaded by default. To load more, use `highlightLanguages`.

A list of all the available styles and languages can be found [here](https://highlightjs.org/static/demo/).

Please note the style and languages should be written in hyphen-separated lowercase, for example:

```toml
[params]
    highlight = true
    highlightStyle = "solarized-dark"
    highlightLanguages = ["go", "haskell", "kotlin", "scala", "swift"]
```
