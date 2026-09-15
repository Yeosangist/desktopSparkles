# Desktop Sparkles
Sparkles for your X11 desktop.<br>
- Five shapes of star
- Editable size, number, frequency, and movement settings
- Fully transparent overlay; shouldn't steal any input
- Lightweight and whimsical

## Install
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
Probably only works on X11. Wayland is fussy about stuff like this.
