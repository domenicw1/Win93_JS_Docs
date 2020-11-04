# $kernel

todo: proper documentation

There is no actual documentation here yet, but $kernel can be used to make something run after boot finished and this page will show you how.

# Run something after boot finished

Anything that does not use this will run during the bios text sequence (which you probably don't want for notifications and windows) before the desktop is loaded.

```js
$kernel.on("splash:ready",function(){
// code here will run on boot
$alert("hello world")
})
```

