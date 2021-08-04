# MinDump Device Dumper
### By FriendlyNeighborhoodShane
*A simple, flexible dumper*

### Links
### Description
This zip dumps all your device partitions into an img format using dd.

It contains a default exclude list which I guess you wouldn't want to dump like system, userdata, cache, etc.

If flashed from recovery, it will take config files from its own directory, make a dumps directory in there and dump everything in it. If flashed from Magisk Manager, it will make a MinDump directory in your internal storage, take configs from there and make a dumps directory to dump stuff.

Config files are:
- mindump-include.txt
- mindump-exclude.txt

A simle list of partitions you want to include or exclude from operation, separated with spaces, newlines or tabs. Only one of them is processed and include takes priority over exclude.

For support:
If you flashed through recovery, provide its logs.
If you used Magisk Manager, provide its logs.

How to control the zip by changing its name:
NOTE: Control by name is not possible in magisk manager, since it copies the zip to a cache directory and renames it install.zip. This is unavoidable behaviour.

- Add 'RESTORE' to its filename to make it restore the dumps it made. WARNING: You really don't want to do this.

Thanks to @osm0sis for the base magisk/recovery code and inspiration and guidance on the majority of the stuff in here. You're awesome.
