# Actually my personal website
# Chirpy Starter

[![Gem Version](https://img.shields.io/gem/v/jekyll-theme-chirpy)](https://rubygems.org/gems/jekyll-theme-chirpy)
[![GitHub license](https://img.shields.io/github/license/cotes2020/chirpy-starter.svg?color=blue)][mit]

The startup template for [**Jekyll Theme Chirpy**][chirpy].

When installing the Chirpy through [RubyGems][gem], Jekyll can only read files in the folders `_includes`, `_layout`, `_sass` and `assets`, as well as a small part of options of the `_config.yml` file from the theme's gem (use the command `bundle info --path jekyll-theme-chirpy` to locate). To fully use all the features of Chirpy, you also need to copy other critical files/directories from the theme's gem to your Jekyll site.

```shell
# The critical files/directories to run Chirpy theme
├── _data
├── _plugins
├── _tabs
├── _config.yml
├── app.js
├── feed.xml
├── index.html
├── robots.txt
├── sw.js
└── 404.html
```

We extracted all the necessary content of **Chirpy** theme's gem to help you quickly use the theme.

## Installation

[Use this template][usetemplate] to generate a new repository, and then execute:

[usetemplate]: https://github.com/cotes2020/chirpy-starter/generate

```
$ bundle
```

## Usage

### Customing Stylesheet

Creare a new file `/assets/css/style.scss` in your Jekyll site.

And then add the following content:

```scss
---
---

@import {{ site.theme }}

// add your style below
```

### Changing the Number of Tabs

When adding or deleting files in the `_tabs` folder, you need to complete the section [Customing Stylesheet](#customing-stylesheet) first, and then add a new line before `@import`:

```scss
$tab-count: {{ site.tabs | size | plus: 1 }};
```

### Publishing to GitHub Pages

See the `jekyll-theme-chirpy`'s [deployment instructions](https://github.com/cotes2020/jekyll-theme-chirpy#deployment). Note that in order to use GitHub Actions caching to speed up the deployment, you should add the `Gemfile.lock` file to your repository.

### Updating

Please note that files and directories in this project may change as the [`jekyll-theme-chirpy`][chirpy] is updated. When updating, please ensure that the file directory structure of your Jekyll site is the same as that of this project.

And then execute:

```console
$ bundle update jekyll-theme-chirpy
```

## Documentation

See the [theme's docs](https://github.com/cotes2020/jekyll-theme-chirpy#documentation).

## License

This work is published under [MIT](mit) License.

[gem]: https://rubygems.org/gems/jekyll-theme-chirpy
[chirpy]: https://github.com/cotes2020/jekyll-theme-chirpy/
[mit]: https://github.com/cotes2020/chirpy-starter/blob/master/LICENSE
