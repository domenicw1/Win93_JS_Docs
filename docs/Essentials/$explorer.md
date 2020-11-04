**This page is not fully complete yet, and several properties are not documented.**

## $explorer

Opens a new file explorer window. Returns an [ExplorerInstance]($explorer.md#explorerinstance).

`$explorer(path)`

| Parameter | Type   | Description                                     |
| --------- | ------ | ----------------------------------------------- |
| path      | String | The path that the explorer should be opened in. |

## ExplorerInstance

Used to represent an explorer window.

| Parameter         | Type                                         | Description                                                  |
| ----------------- | -------------------------------------------- | ------------------------------------------------------------ |
| cfg               | [ExplorerCfg]($explorer.md#explorerinstance) | The configuration of the explorer.                           |
| el                | Array                                        | Array containing HTMLElements of every part of the explorer window. |
| getPath           | Function                                     | Returns the current path of the explorer window.             |
| getSaveInput      | Function                                     | undocumented                                                 |
| getSelectionInput | Function                                     | undocumented                                                 |
| getWindow         | [WinInstance]($window#wininstance)           | Returns the [WinInstance]($window#wininstance) for the explorer window. |
| go                | Function                                     | Navigates the explorer to the specified path.                |
| id                | Integer                                      | The id of the explorer instance.                             |
| refresh           | Function                                     | Reloads the explorer.                                        |
| reorder           | Function                                     | undocumented                                                 |

## ExplorerCfg

Used to represent the configuration of an [ExplorerInstance]($explorer.md#explorerinstance).

| Parameter       | Type     | Description                                               |
| --------------- | -------- | :-------------------------------------------------------- |
| backgroundClass | String   | The classname of the background of the explorer window.   |
| browse          | Boolean  | undocumented                                              |
| footer          | Boolean  | Whether the explorer instance has a footer                |
| id              | Integer  | The id of the explorer instance.                          |
| menu            | Boolean  | Whether the explorer instance has a menu.                 |
| nav             | Boolean  | Whether the explorer instance has a navigation bar.       |
| onclose         | Function | Callback for when the explorer instance is closed.        |
| onopen          | Function | Callback for when the explorer instance is open.          |
| onready         | Function | Callback for when the explorer instance has fully loaded. |
| save            | Boolean  | Whether the window is a "Save File" prompt.               |
| silent          | Boolean  | undocumented                                              |
| viewType        | String   | The view type of the explorer. Can be "icons" or "list".  |

