## $boot
Returns an object containing several things needed for the boot process.

| Parameter | Type        | Description                                                  |
| --------- | ----------- | ------------------------------------------------------------ |
| BIOS      | HTMLElement | The element containing the bios.                             |
| BIOSERROR | HTMLElement | The file name of the zip that's going to be downloaded.      |
| BOOTLOG   | HTMLElement | The element for the text content of the bios.                |
| REINSTALL | HTMLElement | The element for the "Click to reinstall" text that appears when Windows 93 takes too long to boot. |
| TOOLONG   | HTMLElement | The element for the "Boot is taking too long?" text that appears when Windows 93 takes too long to boot. |
| VERSION   | String      | The version of Windows 93 you are currently on.              |
| hasError  | Boolean     | Whether Windows 93 has encountered an error during boot and has interrupted the boot process. |
| onerror   | Function    | The callback for when an error happens during boot.          |