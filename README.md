# Iosevka Nova

Personal customization of the [Iosevka](https://github.com/be5invis/Iosevka) font for my own use.

This variant is mainly based on the JetBrains style, with more curly italics and additional ligatures enabled.

## How to build

1. Ensure that [nodejs](https://nodejs) (≥ 12.16.0) and [ttfautohint](https://www.freetype.org/ttfautohint) are both installed and accessible from `PATH`. 
   Note that the version of nodejs available in the apt package manager might be too old on Ubuntu-based systems.
2. Clone the [Iosevka](https://github.com/be5invis/Iosevka) repo somewhere, e.g. `git clone --depth 1 https://github.com/be5invis/Iosevka`.
3. Copy this repo's `private-build-plans.toml` into the `Iosevka` folder produced by the step above.
4. In that folder, run `npm install` to get all NPM dependencies.
5. Then, run `npm run build -- ttf::iosevka-nova` to build the TTF files.
6. The generated TTF files will be located in `dist/iosevka-nova/`.
