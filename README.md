# VSCode Custom CSS

Custom CSS for VSCode for some visual improvements, just my personal preferences, easily configurable to your liking. Should work okay with most themes, but no guarantees. Only tested on Windows.

## Features

This CSS file adds rounded borders and/or background blur and box shadows to the following elements:

-  IntelliSense suggestions & details widget (two versions, toggleable in `:root`)
-  Parameter hints widget
-  Editor hover tooltips
-  Command palette
-  Files/extensions/etc
-  Minimap slider
-  Breadcrumbs widget
-  Hide the VSCode icon in the title bar

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

## Extra

My changes to the [One Dark Pro Darker](https://marketplace.visualstudio.com/items?itemName=zhuangtongfa.Material-theme) theme to make it just a little nicer. To use, add the following to your `settings.json`:

```json
"workbench.colorCustomizations": {
  "[One Dark Pro Darker]": {
    "editor.background": "#1e2227",
    "sideBar.background": "#191d22",
    "list.inactiveSelectionBackground": "#2d333d",
    "list.hoverBackground": "#2d333d80",
    "titleBar.activeBackground": "#1e2227",
    "sideBarSectionHeader.background": "#1e2227",
    "terminal.background": "#1e2227"
  }
},
"editor.tokenColorCustomizations": {
  "[One Dark Pro Darker]": {
    "comments": "#5c6370",
    "textMateRules": [
      {
        "scope": "comment",
        "settings": {
          "fontStyle": "italic"
        }
      }
    ]
  }
}
```

### Customization tips

Toggle the developer tools from the command palette to view element classes, properties, etc. Use the inspecter to target specific elements.

The JavaScript snippet below can make it easier to inspect elements that don't play nice, just paste it into the console and VSCode will be paused in debug mode after a 3 second delay. Close the developer tools to resume.

```js
setTimeout(function () {
	debugger;
}, 3000);
```
