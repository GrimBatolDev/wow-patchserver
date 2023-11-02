# wow-patchserver

This repo maintains the latest data files that our private server uses.<br>

The patch server folder is structurized as:
- patch-server
    - Patch
        - plist.txt (must have, can be empty)
        - realm.txt (must have)
        - update.txt (must have)
        - wow-launcher.zip (required if we need to update launcher)
        - Patch-X.MPQ
        - Patch-Y.MPQ
        - Patch-Z.MPQ

## plist.txt
This file contains a list of all patch files and their corresponding md5 checksums.<br>
A prefix [XXXX] means this patch should only be used by a specific client.<br>
Currently we only support clients of (enUS, zhCN, zhTW).<br>

Example:<br>
Patch-2.MPQ 32e457c9d18cc1a31d4f9d2429f79a1b<br>
Patch-3.MPQ 1aef7a6f7c17e3e9a426ae5d88273b38<br>
[enUS]Patch-4.MPQ 5912c7916f7b8695b1d5f8f942542d71<br>
[zhCN]Patch-5.MPQ 72e4cc61e22d9360bcb0ebf9cb67492d<br>

## realm.txt
This file contains the IP address of the authserver.<br>

Example:<br>
www.grimbatol-wow.com<br>

## update.txt
This file contains the assembly version number(Major.Minor.Build.Revision) of our latest wow-launcher.<br>

Example:<br>
1.0.0.0<br>

## wow-launcher.zip
This is the archive file of the latest wow-launcher application.<br>
