# Sparkle suite
This was initially limited to the desktop script, but I knew it wasn't the most accessible, so I turned it into a userJS script and an Android app too.<br><br>
The Android app is 5MB, done in Kotlin, and should be nothing on your RAM, but it does need the display over other apps permission. Works for version 5 and above, but only tested on 11.<br><br>
The userJS script should straight up open your userscript manager if you click on the 'Raw'. A quirk that I have observed is that if you navigate away from a page but it stays in memory, when you come back to the page you get a whole BURST of stars, but they clear up pretty quickly, so hopefully it's not too irritating.<br><br>
## Features
- Five shapes of star
- Editable size, number, frequency, and movement settings
- Fully transparent overlay; shouldn't steal any input
- Lightweight and whimsical
- Automatically adapts to light and dark websites (userJS script)
- Permanent notification with stop option (Android APK)

![](https://imgur.com/Bx6uabA.png)

## Install for the desktop script
Enable the script (replace the path with wherever you put it).
```
chmod +x desktop-sparkles.py
```
<br>
REMEMBER TO MODIFY THE SERVICE FILE BEFORE YOU MOVE IT.<br>

```
mv desktop-sparkles.service ~/.config/systemd/user
```
<br>
Reload your system daemon, which should imediately start the script.

```
systemctl --user daemon-reload
systemctl --user enable --now desktop-sparkles.service
```
<br>
Stop the script.

```
systemctl --user stop desktop-sparkles
```
<br>
Restart the script if you modify the configuration.

```
systemctl --user restart desktop-sparkles
```

## Notes
I love free will.<br>
The desktop script has only been tested on X11. Wayland is fussy about stuff like this so idk if it'd work.<br>
Drop a star if you like any of the versions? I just wanna know people are enjoying it.
