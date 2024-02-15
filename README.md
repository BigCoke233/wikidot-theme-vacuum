<h1 align="center">Vacuum</h1>

<p align="center">⚠️ <em>Note that this project is still working in progress.</em> ⚠️</p>

**Vaccum** is a theme for [Wikidot](https://wikidot.com/) written in [Sass](https://sass-lang.com/). Unlike existing wikidot themes, such as [Sigma-9](https://scp-wiki.wikidot.com/sigma-9-themes) and [Black Highlighter](https://scp-wiki.wikidot.com/theme:black-highlighter-theme) (which have been used as the base theme for developing new themes in the SCP Foundation Wiki and Backrooms Wiki), **vacuum is born to a base theme.**

## Usage

Include this line in your Wikidot page.

```
[[module ThemePreviewer noUi="true" theme_url="https://bigcoke233.github.io/wikidot-theme-vacuum/build/vacuum.css"]]
```

## Why Vacuum?

Both Sigma-9 and Black Highlighter are great themes, which inspired a lot of wikidot theme creators. **However, the problem is that they are not created to be modified.** There are quite a lot of fancy effects and preset colors in both themes, making themselves great on the eyes but not a pleasure to build a new style on. 

On one hand, those themes provide an easy and fast way to create a new theme without dealing with the basic layout, letting theme creators focus on the appearance. On the other hand, one has to write certain rules to override existing rules and struggle with CSS priority when using Sigma-9 or BHL as a base.

The most significant issue is that these kind of *overriding* causes a massive amount of CSS rules to be completely useless but browsers still need to handle them, wasting too much resources and thereby lowering performance.

**Vacuum** is a lightweight modular theme, whose core css is only for layout. All the extra style patterns are separated. You can use *vacuum default* (Vacuum Core + Default Styles) or you can use Vacuum Core along with CSS you created!

## Development

If you would like to make contributions to Vacuum, please continute.

### Start Coding

You need to know that Vacuum is written in Sass and built by Parcel (to use parcel's built-in PostCSS support). Also, we use `pnpm` as package manager. So, to develop Vacuum, clone this repository and install dependencies by running the following command.

```
git clone https://github.com/BigCoke233/wikidot-theme-vacuum.git
cd wikidot-theme-vacuum
pnpm install
```

Then, run this command to start dev server.

```
pnpm run dev
```

Make sure you have NodeJS, git, and pnpm installed on your machine.

### Know the Directories

In `./src`, there are all the source sass modules, which cannot be rendered directly by browser.  The core sass files are in `./src/core/` directory while themes like the default one are in other folders.

In `./dist`, there are compiled files built by Parcel. `index.css` contains all core CSS stylesheet, and `index.css.map` is just for browser's dev tools.

You may have noticed the `./build` directory. Well, these are old compiled files, which are no longer in use after we start using Parcel. Thay are likely to be removed in the future.

Vacuum will be adopting monorepo strategy. The `./dist` and `./src` dir will be only for core CSS while themes are separated in another direcotry. Each theme has its own directory which contains their individual `dist` and `src` folder.
