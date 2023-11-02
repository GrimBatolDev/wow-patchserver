# wow-patchserver

This repo maintains the latest data files that our private server uses.

The patch server folder is structurized as:
patch-server
    |
    |- Patch
        | --- plist.txt
        | --- realm.txt
        | --- update.txt
        | --- wow-launcher.zip
        | --- Patch-X.MPQ
        | --- Patch-Y.MPQ
        | --- Patch-Z.MPQ

## plist.txt
This file contains a list of all patch files.
A prefix [XXXX] means this patch should only be used by a specific client.
Currently we only support clients of (enUS, zhCN, zhTW).

Example:
Patch-2.MPQ
Patch-3.MPQ
[enUS]Patch-4.MPQ
[zhCN]Patch-5.MPQ

## realm.txt
This file contains the IP address of the authserver.

Example:
www.grimbatol-wow.com

## update.txt
This file contains the assembly version number(Major.Minor.Build.Revision) of our latest wow-launcher.

Example:
1.0.0.0

## wow-launcher.zip
This is the archive file of the latest wow-launcher application.
