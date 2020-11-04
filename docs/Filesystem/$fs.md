## $fs.utils
An object containing several file system tools. All files are specified using a non-relative path, such as `/a/example.txt`.

| Parameter     | Type     | Description                                                  |
| ------------- | -------- | ------------------------------------------------------------ |
| exist         | Function | Returns false if the specified path doesn't exist, returns the number 0 if the file exists and returns an object if you specify a folder. |
| find          | Function | Returns an array of file paths for every file found. The arguments are the path to start searching from, and the term to search for. |
| getMime       | Function | Returns the mime of the specified file (example: text/plain). |
| getFileName   | Function | Returns the file name (including extension) of the specified file. |
| getFolderName | Function | Returns the folder name of the specified folder path.        |
| getFolderObj  | Function | Returns an object containing the directory path of the specified file path and an object representing the folder containing it. |
| getFolderPath | Function | Returns the path (without the folder itself) to the specified folder. |
| getIcon       | Function | Returns the icon path to the specified file.                 |
| getName       | Function | Returns the file name (including extension) of the specified path. |

