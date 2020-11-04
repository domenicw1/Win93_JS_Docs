## $alert
Shows an alert box that the user can close.

`$alert(options, callback)`

| Parameter | Type     | Description                                                        |
|-----------|----------|--------------------------------------------------------------------|
| options      | String \| [WinObject]($window.md#winobject) | Either the text to display, or a [WinObject]($window.md#winobject) with window options and a msg parameter for the text.                                   |
| callback  | Function | The callback for the function. Called with true if user presses OK |

## $alert.error
Shows an error that the user can close.

`$alert.error(options, callback)`

| Parameter | Type     | Description                                                        |
|-----------|----------|--------------------------------------------------------------------|
| options      | String \| [WinObject]($window.md#winobject) | Either the text to display, or a [WinObject]($window.md#winobject) with window options.                                   |
| callback  | Function | The callback for the function. Called with true if user presses OK |

## $alert.info
Shows an info alert box that the user can close.

`$alert.info(options, callback)`

| Parameter | Type     | Description                                                        |
|-----------|----------|--------------------------------------------------------------------|
| options      | String \| [WinObject]($window.md#winobject) | Either the text to display, or a [WinObject]($window.md#winobject) with window options and a msg parameter for the text.                                  |
| callback  | Function | The callback for the function. Called with true if user presses OK |