# Fedora 45 / GNOME 51 Fix for GJS-OSK Extension

This fix addresses compatibility issues with the **GJS-OSK** GNOME Shell extension on Fedora 45 running GNOME 51.


Update 1: Fixed entering system password bug.
<br>
Update 2: Fixed file renaming bug present in original GJS-OSK release.

## Installation

1. Download the patched `extension.js` file from this repository.

2. Open a terminal and navigate to your GJS-OSK extension directory:

```bash
cd ~/.local/share/gnome-shell/extensions/gjsosk@vishram1123.com/
```

3. Back up your existing file:

```bash
cp extension.js extension.js.backup
```

4. Replace the existing `extension.js` with the downloaded file.

5. Reboot your system:

```bash
sudo reboot
```

After rebooting, GJS-OSK should load the updated extension.

## Restore the Original File

If you encounter problems, restore your backup:

```bash
cd ~/.local/share/gnome-shell/extensions/gjsosk@vishram1123.com/
mv extension.js.backup extension.js
```

Then reboot.

## Compatibility

| Component              | Version / Name              |
|------------------------|-----------------------------|
| Operating System       | Fedora 45                   |
| Desktop Environment    | GNOME 51                    |
| Extension              | GJS-OSK                     |
| Fix                    | Modified `extension.js`     |

## Disclaimer

This is an unofficial community compatibility fix. Always keep a backup of your original extension files before making changes.
