## $cli
Internal function for creating a terminal. **You probably shouldn't use this.** If you need your app to run in the terminal, you should set cli and terminal to true in le._apps or your [app store manifest](../PK93/Introduction.md), or if you just want to open a new terminal, use [$exe("terminal")]($exe.md) instead.

This function is only documented for those trying to create a custom terminal or embedding it directly into their application.

`$cli(e,t)`

| Parameter | Type         | Description                                                  |
| --------- | ------------ | ------------------------------------------------------------ |
| e         | HTMLElement  | Probably the element that the terminal should be appended to? |
| t         | Undocumented | Undocumented                                                 |

