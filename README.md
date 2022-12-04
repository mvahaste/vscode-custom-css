# VSCode Custom CSS

Custom CSS for VSCode for some small improvements, just my personal preferences. Designed with the [One Dark Pro](https://marketplace.visualstudio.com/items?itemName=zhuangtongfa.Material-theme) (Darker) theme in mind.

## Features

This CSS file adds rounded borders and/or background blur and box shadows to the following elements:

-  IntelliSense suggestions box
-  Editor hover tooltips
-  Command palette
-  Files/extensions/etc
-  Minimap slider

It also resizes the window controls to be square.

## Installation

Install the [Custom CSS and JS Loader](https://marketplace.visualstudio.com/items?itemName=be5invis.vscode-custom-css) extension.

Add the following to your `settings.json`:

```json
"vscode_custom_css.imports": [
  "file:///path/to/vscode-custom-css/custom.css"
],
```
