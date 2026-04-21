# Ares Themed Roller for Game Pad Viewer

Use [This Link](https://app.gpv.gg/?p=1&s=5&editcss=https%3A%2F%2Fsonsofares.github.io%2Fgamepad-viewer%2Fds4%2Fedit.css&dz=0.01&soffset=25) in your OBS browser scene.

## View Assets

Use [This Link](https://sonsofares.github.io/gamepad-viewer/ds4/index.html) to view the assets.

## Permissions in OBS

To add the `--disable-features=EnableWindowsGamingInputDataFetcher` command to OBS Studio on startup (often used to fix controller/input overlay issues), you need to modify the OBS shortcut in the Windows Startup folder.

### Step-by-Step Instructions

1. Create/Locate the OBS Shortcut:
    - If OBS is not a shortcut on your Desktop, search for "OBS Studio" in the Start Menu, right-click it, and select Open file location.
    - Right-click the `OBS Studio` shortcut, select Copy, and then Paste it onto your Desktop.
2. Modify the Shortcut:
    - Right-click the `OBS Studio` shortcut on your Desktop and select Properties.
    - Go to the **Shortcut** tab.
    - In the **Target** field, go to the very end of the text, add a space, and then paste the following command:
`--disable-features=EnableWindowsGamingInputDataFetcher`
3. Apply and Restart:
    - Click **Apply** and then **OK**.
    - Restart your computer to test if OBS launches with the command applied. 


The target line should look something like this:

```
"C:\Program Files\obs-studio\bin\64bit\obs64.exe" --disable-features=EnableWindowsGamingInputDataFetcher
```
