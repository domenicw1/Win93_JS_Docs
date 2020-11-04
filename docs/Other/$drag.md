# $drag

Makes an element draggable. Used internally for icons.

`$drag(element, options)`

| Parameter | Type                             | Description                     |
| --------- | -------------------------------- | ------------------------------- |
| element   | HTMLElement                      | The element to become draggable |
| options   | [DragOptions]($drag#DragOptions) | The options for the dragging.   |

# DragOptions

The options for the dragging. All parameters are optional.

| Parameter | Type        | Description                                                  |
| --------- | ----------- | ------------------------------------------------------------ |
| constrain | Boolean     | Whether the draggable icon goes back to its original positions after you stop dragging |
| ghost     | Boolean     | Whether the icon is a ghost                                  |
| grid      | Boolean     | Whether the icon is forced to a grid                         |
| handle    | HTMLElement | The handle that the icon is dragged from. This is optional.  |
| distance  | Integer     | I'm not sure what this does.                                 |
| oninit    | Function    | Called when the icon is first made draggable                 |
| onstart   | Function    | Called when someone starts dragging the icon                 |
| ondrag    | Function    | Called when an icon is being moved                           |
| onstop    | Function    | Called when someone stops dragging an icon                   |

