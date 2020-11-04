# $el

Returns the [ElObject]($el#ElObject) of a HTMLElement

`$el(element)`

| Parameter | Type        | Description                                           |
| --------- | ----------- | ----------------------------------------------------- |
| element   | HTMLElement | The element to turn into an [ElObject]($el#ElObject). |



# $el.create

Create a new element. Works similarly to `document.createElement`. Returns a HTMLElement

`$el.create(selector)`

| Parameter | Type   | Description                                                  |
| --------- | ------ | ------------------------------------------------------------ |
| selector  | String | The css selector of the new element to create. Example: You can use `div` to create a div, `div#test` to create a div with the id test, and `div.test` to create a div with the class test. |

# $el.each

Loops over every element in the entire document with a specific selector

`$el.each(selector,cb)`

| Parameter | Type     | Description                                                  |
| --------- | -------- | ------------------------------------------------------------ |
| selector  | String   | The css selector of what elements to loop over. Example: for every single div, use `div` and for every single div with the class test, use `div.test` |
| cb        | Function | Called (with the HTMLElement) once for every single element matching the selector. |



# ElObject

Object representing an $el element.

| Parameter | Type                          | Description                                             |
| --------- | ----------------------------- | ------------------------------------------------------- |
| add       | Function (param: String)      | Appends text (or html) to the innerHTML of the element. |
| append    | Function (param: HTMLElement) | Appends                                                 |
| click     | Function                      | Simulates a click on the element                        |
| each      | Function                      | See [$el.each]($el.md#$el.each)                         |
| get       | Function                      | Returns the HTMLElement                                 |
| html      | Function                      | Returns the HTML of the element as a string.            |
| off       | Function                      | Event stuff - todo: document                            |
| on        | Function                      | Event stuff - todo: document                            |

