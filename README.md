# Lanyon for Leafpub

[Lanyon](https://github.com/poole/lanyon) is a theme built by [mdo](https://github.com/mdo), originally for [Jekyll](http://jekyllrb.com/). This repository is a conversion of that theme to work with [Leafpub](https://www.leafpub.org/).

## Contents

- [Usage](#usage)
- [Options](#options)
  - [Themes](#themes)
  - [Reverse layout](#reverse-layout)
- [Development](#development)
- [Author](#author)
- [License](#license)

## Options

Lanyon includes some customizable options, typically applied via classes on the `<body>` element.

### Themes

Lanyon ships with eight optional themes based on the [base16 color scheme](https://github.com/chriskempson/base16). Apply a theme to change the color scheme (mostly applies to sidebar and links).

![Lanyon with red theme](https://f.cloud.github.com/assets/98681/1825270/be065110-71b0-11e3-9ed8-9b8de753a4af.png)
![Lanyon with red theme and open sidebar](https://f.cloud.github.com/assets/98681/1825269/be05ec20-71b0-11e3-91ea-a9138ef07186.png)

There are eight themes available at this time.

![Available theme classes](https://f.cloud.github.com/assets/98681/1817044/e5b0ec06-6f68-11e3-83d7-acd1942797a1.png)

To use a theme, add any one of the available theme classes to the `<body>` element in the `default.hbs` layout, like so:

```html
<body class="theme-base-08">
  ...
</body>
```

To create your own theme, look to the Themes section of `lanyon.css`. Copy any existing theme (they're only a few lines of CSS), rename it, and change the provided colors.


### Reverse layout

![Lanyon with reverse layout](https://f.cloud.github.com/assets/98681/1825265/be03f2e4-71b0-11e3-89f1-360705524495.png)
![Lanyon with reverse layout and open sidebar](https://f.cloud.github.com/assets/98681/1825268/be056174-71b0-11e3-88c8-5055bca4307f.png)

Reverse the page orientation with a single class.

```html
<body class="layout-reverse">
  ...
</body>
```


### Sidebar overlay instead of push

Make the sidebar overlap the viewport content with a single class:

```html
<body class="sidebar-overlay">
  ...
</body>
```

This will keep the content stationary and slide in the sidebar over the side content. It also adds a `box-shadow` based outline to the toggle for contrast against backgrounds, as well as a `box-shadow` on the sidebar for depth.

It's also available for a reversed layout when you add both classes:

```html
<body class="layout-reverse sidebar-overlay">
  ...
</body>
```

### Sidebar open on page load

Show an open sidebar on page load by modifying the `<input>` to add the `checked` boolean attribute:

```html
<input type="checkbox" class="sidebar-checkbox" id="sidebar-checkbox" checked>
```

## Development

Lanyon has two branches, but only one is used for active development.

- `master` for development.  **All pull requests should be to submitted against `master`.**
- `gh-pages` for our hosted site, which includes our analytics tracking code. **Please avoid using this branch.**


## Author

**Mark Otto** - creator
- <https://github.com/mdo>
- <https://twitter.com/mdo>

**Daniel Jost** - Ghost fork
- <https://github.com/PxlBuzzard>
- <https://twitter.com/_danieljost_>

**Cory LaViska** - Leafpub fork
- <https://www.leafpub.org/>
- <https://twitter.com/leafpub>

## License

Open sourced under the [MIT license](LICENSE.md).
