# $log

Writes text in the terminal. This should be used in terminal/cli apps to show information. You can use html in the text parameter for more specific styling.

`$log(text)`

| Parameter | Type   | Description                            |
| --------- | ------ | -------------------------------------- |
| text      | String | The text to be written in the terminal |

### Styling

**$log.pass** - logs text in green with a checkmark before it

**$log.fail** - logs text in red with a cross before it

**$log.bold** - logs text in bold

**$log.italic** - logs text in italic

**$log.code** - logs text with a codeblock background

**$log.error** - logs text in red

**$log.succes** - logs test in green

**$log.any_color** - logs text in a specific color, works for most colors

