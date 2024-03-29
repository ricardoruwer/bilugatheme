# Biluga Theme

Basic VSCode dark theme

## Installation

You can install it through the [VSCode Marketplace](https://marketplace.visualstudio.com/items?itemName=ricardoruwer.bilugatheme).

## Activation

Press `⌘K ⌘T` and select `BilugaTheme` on the list.

## Screenshots

It's just a simple screenshot from an Elixir code. You have to try the theme to see all the colors.

![Elixir](https://ricardoruwer.s3.amazonaws.com/Rh0M776S.png)

## Some cool settings

```js
{
  // ...
  "editor.fontFamily": "OperatorMono-Book",
  "editor.lineHeight": 28,
  // https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme
  "workbench.iconTheme": "material-icon-theme",
  // And some other I use, you can see here: https://gist.github.com/ricardoruwer/b67986152b239fb27ffb488d156de7d3#file-settings-json
  // ...
}
```

## Override colors

You can override some of the theme colors if you want, to do that you can follow [this doc](https://code.visualstudio.com/docs/getstarted/themes#_customizing-a-color-theme).
To know the name of the textmate scope, press `⌃ ⇧ P`.

### Example

```js
{
  // ...
  "workbench.colorCustomizations": {
    "editor.background": "#1A202C",
    "editor.foreground": "#EDF2F7",
    // ...
  },
  "editor.tokenColorCustomizations": {
    "textMateRules": [
      {
        "scope": [
          "comment"
        ],
        "settings": {
          "fontStyle": "italic",
          "foreground": "#4A5568"
        }
      },
      // ...
    ]
  }
  // ...
}
```

## Publish extension
You can use the [`vsce`](https://www.npmjs.com/package/vsce) extension to publish the extension on the Marketplace, example:
```bash
vsce publish 1.1.4
```
Click [here](https://code.visualstudio.com/api/working-with-extensions/publishing-extension) to know more.
