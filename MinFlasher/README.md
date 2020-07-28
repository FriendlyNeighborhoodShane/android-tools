# Minimal Flasher
### By FriendlyNeighborhoodShane
*A simple zip to flash all zips*

### Links
* [Support](https://t.me/joinchat/FyFlS0X2D7f6YNvdxhEsfw)
### Description
This zip flashes all the zips in a directory. It can be flashed in either recovery or Magisk Manager.

If you flash the zip from Magisk Manager, it can only install Magisk-compatible zips (zips that could have been flashed normally from MM). From recovery, it will flash all zips.

For support:
If you flashed through recovery, provide its logs.
If you used Magisk Manager, provide its logs.

How to control the zip:
NOTE: Control by name is not possible in magisk manager, since it copies the zip to a cache directory and renames it install.zip. This is unavoidable behaviour.

- Add 'silent' to its filename to not show you the output from each of the individual zips on the UI. Otherwise, it shows all output.

- The zip will flash zips from the first directory in which it finds zip files (in decreasing order of preference):
-- Inside the zip in "Zips" folder
-- [Zip's directory]                            (only useable in recovery mode)
-- internal-storage/MinFlasher        (use in recovery mode only if MinFlasher is in this directory)

- You can control the order in which it flashes zips by name. It flashes all zips alphabetically, in order ")-.[0-9]_[A-Z][a-z]("

Thanks to @osm0sis for the base magisk/recovery code, the base flashing script and inspiration and guidance on the majority of the stuff in here. You're awesome.
