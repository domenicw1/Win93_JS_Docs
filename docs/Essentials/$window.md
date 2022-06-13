## $window

Creates and opens a new window.

`$window(options)`

| Parameter | Type                    | Description                 |
| --------- | ----------------------- | --------------------------- |
| options   | [WinObject](#winobject) | The options for the window. |

## $window.instances

Contains a [WinInstance]($window#wininstance) array of all open windows.

## $window.current

Function that returns the [WinInstance]($window#wininstance) of the current focused window.

## $window.form

Creates and opens a window containing a form.

`$window.form(form,callback)`

| Parameter | Type   | Description                                                  |
| --------- | ------ | ------------------------------------------------------------ |
| form      | String | An object representing the form, where property names are form fields and property values are form values. See [examples](../examples.md) |
| callback  | String | The object specified above, except with the values modified by the user. |

## $window.active

Makes the specified window id active/focused.

`$window.active(id)`

| Parameter | Type    | Description                                                  |
| --------- | ------- | ------------------------------------------------------------ |
| id        | Integer | The id of the window, found in a [WinInstance]($window#wininstance). |

## $window.close

Closes the specified window id

`$window.close(id)`

| Parameter | Type    | Description                                                  |
| --------- | ------- | ------------------------------------------------------------ |
| id        | Integer | The id of the window, found in a [WinInstance]($window#wininstance). |

## $window.destroy

Destroys the specified window id (no animation, calls ondestroy)

`$window.destroy(id)`

| Parameter | Type    | Description                                                  |
| --------- | ------- | ------------------------------------------------------------ |
| id        | Integer | The id of the window, found in a [WinInstance]($window#wininstance). |

## $window.maximize

Toggles whether the specified window id is maximzied

`$window.maximize(id)`

| Parameter | Type    | Description                                                  |
| --------- | ------- | ------------------------------------------------------------ |
| id        | Integer | The id of the window, found in a [WinInstance]($window#wininstance). |

## $window.restore

Restores a minimized window. Warning: this will throw an error if the specified window is not minimized.

`$window.maximize(id)`

| Parameter | Type    | Description                                                  |
| --------- | ------- | ------------------------------------------------------------ |
| id        | Integer | The id of the window, found in a [WinInstance]($window#wininstance). |

## WinObject

The object containing the options for a window. Can also be used with [$alert]($alert.md). **Every parameter is optional.**

| Parameter    | Type     | Description                                                  |
| ------------ | -------- | ------------------------------------------------------------ |
| url          | String   | The url that the window should iframe. (this only works with urls that allow it) |
| title        | String   | The title of the window.                                     |
| width        | Integer  | The width of the window in pixels.                           |
| height       | Integer  | The height of the window in pixels.                          |
| html         | String   | The html that the window should contain.                     |
| icon         | String   | Path to the icon of the window.                              |
| msg          | String   | This is only for $alert - The text it should display.        |
| header       | Boolean  | Whether the window titlebar is visible.                      |
| resizable    | Boolean  | Whether the window can be resized.                           |
| maximizable  | Boolean  | Whether the window can be maximized.                         |
| minimizable  | Boolean  | Whether the window can be minimized.                         |
| draggable    | Boolean  | Whether the window can be dragged around.                    |
| closable     | Boolean  | Whether the window can be closed.                            |
| dockable     | Boolean  | Whether the window appears on the taskbar.                   |
| center       | Boolean  | Whether the window is centered.                              |
| automaximize | Boolean  | Whether the window is automatically maximized.               |
| help         | String   | The help string that appears when the help button is pressed. |
| menu         | MenuArr  | The menu at the top of the window.                           |
| footer       | String   | The text that is at the bottom of a window.                  |
| contextmenu  | MenuArr  | Menu documentation is not finished yet.                      |
| animationIn  | String   | The animation name (from animate.css) for when you open the window. |
| animationOut | String   | The animation name (from animate.css) for when you close the window. |
| onactive     | Function | Callback for when window becomes active (gets clicked on).   |
| oncancel     | Function | Callback for when the cancel button is pressed.              |
| onclose      | Function | Callback for when the window is closed.                      |
| ondestroy    | Function | Callback for when the window is destroyed (using killall or $window.instances). |
| ondrag       | Function | Callback for when the window is being dragged.               |
| ondragstop   | Function | Callback for when the window stops being dragged.            |
| onminimize   | Function | Callback for when the window has been minimized.             |
| onok         | Function | Callback for when the OK button has been pressed.            |
| onopen       | Function | Callback for when the window is opened.                      |
| onready      | Function | Callback for when the window is fully loaded.                |

## WinInstance

Object representing an open window

| Parameter    | Type                    | Description                                                  |
| ------------ | ----------------------- | ------------------------------------------------------------ |
| active       | Function                | Returns whether the window is currently active/selected.     |
| cfg          | [WinObject](#winobject) | Returns the WinObject of the window.                         |
| changeFooter | Function                | Changes the footer of the window (text).                     |
| changeIcon   | Function                | Changes the icon of the window (icon path).                  |
| changeSize   | Function                | Changes the size of the window (width, height).              |
| changeTitle  | Function                | Changes the title of the window (text).                      |
| close        | Function                | Closes the window (playing the animation and calls onclose). |
| destroy      | Function                | Destroys a window (no animation, ondestroy is called).       |
| el           | Object                  | Object containing HTMLElements for all parts of the window.  |
| id           | Integer                 | The ID of the window.                                        |
| maximize     | Function                | Maximizes the window.                                        |
| menu         | MenuArr                 | Returns the menu of a window (documentation not finished).   |
| minimize     | Function                | Minimizes a window.                                          |
| restore      | Function                | Restores a minimized window.                                 |


## MenuArr

Array of dropdown menu items.

| Parameter    | Type      | Description                                                  |
| ------------ | --------- | ------------------------------------------------------------ |
| name         | String    | The name of the menu item.                                   |
| items        | MenuItem[]| The items in the menu.                                       |

## MenuItem

| Parameter    | Type      | Description                                                  |
| ------------ | --------- | ------------------------------------------------------------ |
| name         | String    | The name of the menu item.                                   |
| action	   | Function  | The function to call when the menu item is clicked.          |