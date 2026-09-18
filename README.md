# Sparkle suite
Sparkles for your [desktop](https://github.com/Yeosangist/sparkleSuite/raw/refs/heads/main/desktop-sparkles.py), [browser](https://github.com/Yeosangist/sparkleSuite/raw/refs/heads/main/web-sparkles.user.js), and [Android](https://github.com/Yeosangist/sparkleSuite/raw/refs/heads/main/sparkles.apk).<br><br>
![](https://imgur.com/6y2hyn3.gif)<br><br>
Because we all deserve more sparkles in our life.

## Features
- Five star shapes
- Editable size, number, frequency, and movement settings
- Fully transparent overlay; shouldn't steal any input
- Lightweight and whimsical
- Automatically adapts to light and dark websites (userscript)
- Permanent notification with a stop option (Android APK)

## Install - Desktop script
Make the script executable:
```
chmod +x desktop-sparkles.py
```
<br>
<b>REMEMBER TO MODIFY THE SERVICE FILE BEFORE YOU MOVE IT.</b><br>
Move the service file to your user systemd directory:

```
mv desktop-sparkles.service ~/.config/systemd/user/
```
<br>
Reload the systemd user daemon and start the service:

```
systemctl --user daemon-reload
systemctl --user enable --now desktop-sparkles.service
```
<br>
Stop the script:

```
systemctl --user stop desktop-sparkles.service
```
<br>
Restart the script if you modify the configuration:

```
systemctl --user restart desktop-sparkles.service
```

## Notes
I love free will.<br><br>
The desktop script has only been tested on X11. Wayland is fussy about stuff like this so I have no idea if it'll work there.<br><br>
My laptop is 10+ years old and has an integrated graphics card, and running the script only has a 3% increase on my CPU usage, so yeah. It's light.<br><br>
The Android app is 5MB, done in Kotlin, and should have a minimal RAM footprint. It does require the <b>display over other apps</b> permission.<br><br>
Theoretically, the app works on Android version 5 and above, but it has only tested on Android 11.<br><br>
The userscript should open your userscript manager when you click <b>'[Raw](https://github.com/Yeosangist/sparkleSuite/raw/refs/heads/main/web-sparkles.user.js)'</b>.<br><br>
Drop a star if you like any of the versions! I just wanna know people are enjoying it.
