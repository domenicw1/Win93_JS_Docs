## $notif
Shows a taskbar notification

`$notif(options)`

| Parameter | Type     | Description                                                                                            |
|-----------|----------| ------------------------------------------------------------------------------------------------------ |
| options | String \| [NotifObject]($notif#notifobject) | The options for the notification. If a string is specified, it will show it. |

## NotifObject

An object containing the properties of a notification.

| Parameter         | Type    | Description                                                  |
| ----------------- | ------- | ------------------------------------------------------------ |
| msg               | String  | The text shown in the notification.                          |
| title (optional)  | String  | The title shown above the text in the notification.          |
| img (optional)    | String  | The path to the image shown next to the text.                |
| length (optional) | Integer | The number of milliseconds the notification should be shown for. |

