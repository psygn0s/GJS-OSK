Fedora 45 / GNOME 51 Fix for GJS-OSK Extension

This fix addresses compatibility issues with the GJS-OSK GNOME Shell extension on Fedora 45 running GNOME 51.

Installation: 
Download the patched extension.js file from this repository.
Open a terminal.
Navigate to your GJS-OSK extension directory:
```console
cd ~/.local/share/gnome-shell/extensions/gjsosk@vishram1123.com/
```
Back up your existing file:
```console
cp extension.js extension.js.backup
```
Replace the existing extension.js with the downloaded file.
Reboot your system.

```console
sudo reboot
```

After rebooting, GJS-OSK should load the updated extension.

Restore the Original File

If you encounter problems, restore your backup:

```console
cd ~/.local/share/gnome-shell/extensions/gjsosk@vishram1123.com/
mv extension.js.backup extension.js
```


Then reboot.

Compatibility
Operating System: Fedora 45
Desktop Environment: GNOME 51
Extension: GJS-OSK
Fix: Modified extension.js
Disclaimer

This is an unofficial community compatibility fix. Always keep a backup of your original extension files before making changes.
