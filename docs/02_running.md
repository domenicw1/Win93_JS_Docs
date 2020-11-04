# Running your apps

There are 4 ways to run a script on the website. The recommended way for development is using the DevTools as they are made for that purpose and make it easy to access functions.

# DevTools

Pressing Ctrl+Shift+I with the website open in your browser, should make the Dev Tool Panel show up. To access the console where you will run your script, you need to press on the `Console` button at the top. You can then start writing code or paste in your script, and by pressing Enter it should run immediately.

![Image of Dev Tools Panel](https://cdn.discordapp.com/attachments/699354946050457730/773655599161802762/unknown.png)

# Boot folder

Any JS or CSS file located in /a/boot will be ran every time Windows 93 boots. You can press anywhere on the screen during the boot process to trigger the BIOS and go into Safe Mode if any script messes up the boot process.

Please note that any scripts in that folder will run during the boot sequence, which can mess up your script. It is highly recommended to wrap your scripts with an event handler for the boot sequence being finished, like this:

```js
$kernel.on("splash:ready",function(){
// code here will run on boot
$alert("hello world")
})
```





# Terminal

Pasting code in the Windows 93 Terminal is going to run it and return the output.

![Terminal](https://cdn.discordapp.com/attachments/699354946050457730/773657050919600128/unknown.png)

# JS Application

By using the `js` app in the terminal, you can run any JS file you've saved on Windows 93

![js](https://cdn.discordapp.com/attachments/699354946050457730/773657582703083541/unknown.png)

