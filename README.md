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