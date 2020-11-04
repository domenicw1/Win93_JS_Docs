## $prompt
Shows a prompt window that the user can input text into.

`$prompt(text, placeholder, callback)`

| Parameter   | Type     | Description                                                  |
| ----------- | -------- | ------------------------------------------------------------ |
| text        | String   | The question shown in the prompt                             |
| placeholder | String   | The text already entered in the input box. This is required, use an empty string if not needed. |
| callback    | Function | The callback. Called with two arguments, whether the user has pressed OK and the text they entered. |