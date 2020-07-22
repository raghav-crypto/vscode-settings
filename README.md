# VS Code Settings (For Web Dev)

# Font

* [Anonymous Pro](https://www.marksimonson.com/fonts/view/anonymous-pro)

# Extensions
See my full list of Extenstions [here](https://gist.github.com/raghav-crypto/ca3c627d30e40a1436284980afff8b42)

## Themes/Color

* [Seti-Black](https://marketplace.visualstudio.com/items?itemName=bobsparadox.seti-black)
* [Material Icon Theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme)
* [Bracket Pair Colorizer](https://marketplace.visualstudio.com/items?itemName=coenraads.bracket-pair-colorizer)

## Workflow

* [advanced-new-file](https://marketplace.visualstudio.com/items?itemName=patbenatar.advanced-new-file)
  * Adds the ability to create files anywhere in your workspace.
* [Auto Rename Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag)
  * Automatically rename paired HTML/XML tag

## IntelliSense/AutoComplete

* [npm Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.npm-intellisense)
  * Autocompletes npm modules in import/require statements
* [Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense)
  * Autocompletes filenames

## Style/Formatting

* [Beautify](https://marketplace.visualstudio.com/items?itemName=hookyqr.beautify)
  * Automatically format javascript, JSON, CSS, Sass, and HTML files.

# Settings

```json
{
  "editor.fontFamily": "\"Anonymous Pro\"",
  "window.zoomLevel": 1,
  "editor.renderLineHighlightOnlyWhenFocus": true,
  "editor.renderIndentGuides": false,
  "editor.matchBrackets": false,
  "editor.snippetSuggestions": "top",
  "editor.renderWhitespace": "none",
  "editor.formatOnPaste": true,
  "files.autoSave": "off",
  "editor.tabSize": 2,
  "editor.lineHeight": 0,
  "editor.fontSize": 14,
  "advancedNewFile.exclude": {
    "node_modules": true,
    "node_modules_electron": true,
    "dev": true,
    "dist": true
  },
  "advancedNewFile.showInformationMessages": true,
  "advancedNewFile.convenienceOptions": ["last", "current", "root"],
  "[json]": {
    "editor.quickSuggestions": {
      "strings": true
    },
    "editor.suggest.insertMode": "replace"
  },
  "[javascript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "workbench.iconTheme": "material-icon-theme",
  "window.menuBarVisibility": "toggle",
  "workbench.statusBar.visible": false,
  "workbench.activityBar.visible": false,
  "editor.minimap.enabled": false,
  "[html]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "emmet.includeLanguages": {
    "javascript": "javascriptreact"
  },
  "emmet.triggerExpansionOnTab": true,
  "[jsonc]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "explorer.confirmDelete": false,
  "liveSassCompile.settings.formats": [
    {
      "format": "expanded",
      "extensionName": ".css",
      "savePath": "dist/css"
    }
  ],
  "liveServer.settings.donotShowInfoMsg": true,
  "material-icon-theme.folders.theme": "specific",
  "workbench.colorTheme": "Seti Black",
  "workbench.colorCustomizations": {
    "activityBarBadge.background": "#FF7042",
    "activityBar.activeBorder": "#FF7042",
    "list.activeSelectionForeground": "#FF7042",
    "list.inactiveSelectionForeground": "#FF7042",
    "list.highlightForeground": "#FF7042",
    "scrollbarSlider.activeBackground": "#FF704250",
    "editorSuggestWidget.highlightForeground": "#FF7042",
    "textLink.foreground": "#FF7042",
    "progressBar.background": "#FF7042",
    "pickerGroup.foreground": "#FF7042",
    "tab.activeBorder": "#FF7042",
    "notificationLink.foreground": "#FF7042",
    "editorWidget.resizeBorder": "#FF7042",
    "editorWidget.border": "#FF7042",
    "settings.modifiedItemIndicator": "#FF7042",
    "settings.headerForeground": "#FF7042",
    "panelTitle.activeBorder": "#FF7042",
    "breadcrumb.activeSelectionForeground": "#FF7042",
    "menu.selectionForeground": "#FF7042",
    "menubar.selectionForeground": "#FF7042",
    "editor.findMatchBorder": "#FF7042",
    "selection.background": "#FF704240",
    "statusBarItem.remoteBackground": "#FF7042"
  },
  "materialTheme.accent": "Orange",
  "breadcrumbs.enabled": true
}
```

# Keybindings
***For Better Control Over Keyboard, Some Overrides***
```json
[
  { "key": "ctrl+j", "command": "cursorDown", "when": "textInputFocus" },
  { "key": "ctrl+k", "command": "cursorUp", "when": "textInputFocus" },
  {
    "key": "shift+v",
    "command": "cursorDownSelect",
    "when": "textInputFocus"
  },
  {
    "key": "ctrl+shift+j",
    "command": "cursorDownSelect",
    "when": "textInputFocus"
  },
  {
    "key": "ctrl+shift+k",
    "command": "cursorUpSelect",
    "when": "textInputFocus"
  },
  {
    "key": "ctrl+shift+h",
    "command": "cursorWordStartLeftSelect",
    "when": "textInputFocus"
  },
  {
    "key": "ctrl+shift+l",
    "command": "cursorWordStartRightSelect",
    "when": "textInputFocus"
  },
  {
    "key": "ctrl+l",
    "command": "cursorWordEndRight",
    "when": "textInputFocus"
  },
  {
    "key": "ctrl+h",
    "command": "cursorWordStartLeft",
    "when": "textInputFocus"
  }
]

```
