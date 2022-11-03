# Examples

These are pieces of code that you can look at to further understand how to use specific functions.

**Do not copy these.** These examples are made for you to learn from, not to steal. If your app is one of the examples with only a few lines of code changed, it's probably not a good app. Try following our beginners guide instead.

# Running something when boot is properly finished

If you're running scripts in /a/boot, this is required for some things to function properly as scripts usually run during the boot sequence, not after it.

```js
$kernel.on("splash:ready",function(){
// Your code goes here and will be ran after boot finishes
$alert("hello world")
})
```

# Confirmation Prompt

This uses the callback from $prompt that gets called with a boolean indicating whether the user pressed OK or not.

```js
$confirm('Are you sure you want to do this?', function (ok){
  if (ok) {
    $alert('You pressed OK.')
  } else {
    $alert('You pressed Cancel.')
  }
});
```

# Proper Alert Order using Callbacks

This is another example of how to properly use callbacks to do things in a proper sequence.

```js
$alert("This will show first!",function(){
    $alert("This will show second!",function(){
        $alert("This will show third!")
    }
})
```

# Window with text inside that can't be resized

This is an example of how to use [$window](./Essentials/$window.md) together with a [WinObject](./Essentials/$window.md#winobject) to properly create and customize a window.

```js
$window({
	title: "My window",
	html: "Hello world!",
	icon: "/c/sys/skins/w93/apps/hexedit.png",
    resizable: false,
    maximizable: false
})
```

# Getting the text from a prompt

This uses a callback that has two parameters to get the text from a prompt.

```javascript
$prompt('What is your name?', '', function(ok, text) {
  if (ok) {
    $alert("Hello, " + text)
  }
});
```

# File Selection

This is an example of how to properly use $explorer to create a file selection dialog.

```js
$explorer('a/', {browse: true, explorer: true, onclose: function(ok, file) {
  if(ok){
  	$alert("Selected file path " + file);
  }else{
  	$alert("User has cancelled")
  }
}});
```

