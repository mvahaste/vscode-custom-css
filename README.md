# VSCode Custom CSS

Custom CSS for VSCode for some small improvements, just my personal preferences, easily configurable to your liking. Should work okay with most themes, but no guarantees. Only tested on Windows.

## Features

This CSS file adds rounded borders and/or background blur and box shadows to the following elements:

-  IntelliSense suggestions widget (two versions, toggleable in `:root`)
-  Parameter hints widget
-  Editor hover tooltips
-  Command palette
-  Files/extensions/etc
-  Minimap slider

It also resizes the window controls to be square.

## Screenshots

<details>
  <summary>Suggest widget (1)</summary>

![Suggest Widget (1)](/screenshots/suggest-widget-1.png)

</details>

<details>
  <summary>Suggest widget (0)</summary>

![Suggest Widget (0)](/screenshots/suggest-widget-0.png)

</details>

<details>
  <summary>Parameter hint</summary>

![Parameter hint](/screenshots/tooltip.png)

</details>

<details>
  <summary>GitLive tooltip</summary>

![GitLive tooltip](/screenshots/gitlive-tooltip.png)

</details>

<details>
  <summary>Command palette</summary>

![Command palette](/screenshots/command-palette.png)

</details>

Screenshots are taken with the [Github Dark](https://marketplace.visualstudio.com/items?itemName=GitHub.github-vscode-theme) theme.

## Installation

Install the [Custom CSS and JS Loader](https://marketplace.visualstudio.com/items?itemName=be5invis.vscode-custom-css) extension.

Add the following to your `settings.json`:

```json
"vscode_custom_css.imports": [
  "file:///path/to/vscode-custom-css/custom.css"
],
```
