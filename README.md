# Edition

The newsletter theme for [Ghost](http://github.com/tryghost/ghost/). This is the latest development version of Edition! If you're just looking to download the latest release, head over to the [releases](https://github.com/TryGhost/Edition/releases) page.

# Edition Translations Fork

This fork contains translations for English, German and Turkish. If you want to add a new language just copy one of the files in the `locales` folder, rename it to your language string (e.g. `es.json` for Spanish) and replace the values with the translated strings. After that, follow the Development instructions below to generate the zip and upload it to your site. Finally, make sure to set the language in your Ghost Dashboard correctly (Settings > General > Publication Language)

I'm happy to accept PRs with translations of new languages.

&nbsp;

# Development

Edition styles are compiled using Gulp/PostCSS to polyfill future CSS spec. You'll need [Node](https://nodejs.org/), [Yarn](https://yarnpkg.com/) and [Gulp](https://gulpjs.com) installed globally. After that, from the theme's root directory:

```bash
# Install
yarn

# Run build & watch for changes
$ yarn dev
```

Now you can edit `/assets/css/` files, which will be compiled to `/assets/built/` automatically.

The `zip` Gulp task packages the theme files into `dist/<theme-name>.zip`, which you can then upload to your site.

```bash
# create .zip file
yarn zip
```

# PostCSS Features Used

- Autoprefixer - Don't worry about writing browser prefixes of any kind, it's all done automatically with support for the latest 2 major versions of every browser.

# Copyright & License

Copyright (c) 2013-2021 Ghost Foundation - Released under the [MIT license](LICENSE).
