## $confirm
Shows a confirmation alert box that the user can close. The same as $alert, except with a question mark icon and a OK and Cancel button, where the OK buttons returns true in a callback

`$confirm(options, callback)`

| Parameter | Type     | Description                                                        |
|-----------|----------|--------------------------------------------------------------------|
| options      | String \| [WinObject]($window.md#winobject) | Either the text to display, or a [WinObject]($window.md#winobject) with window options and a msg parameter for the text.                                   |
| callback  | Function | The callback for the function. Called with true if user presses OK, and with false if the user pressed Cancel. |
