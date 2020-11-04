# The Filesystem

The file system is the /a/ drive, found on the Windows 93 desktop. 

This is the place where you'll be storing any files. Your application, configuration, and any other things you may need are all stored there. 

Windows 93 uses 2 file systems combined to create /a/, and there are three different functions to access them.

## Relative Paths

**This only applies to $store and $db, you do need to include the /a/ when using $file**

File paths are relative to /a/. This means, if you want to read /a/hey/test.txt, instead of writing `$db.get("/a/cool/file.txt")`, you would write `$db.get("cool/file.txt")` instead. This does not apply to $file.

## Which function should I use for saving files?

todo