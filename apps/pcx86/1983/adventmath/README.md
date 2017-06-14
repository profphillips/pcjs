---
layout: page
title: "Adventures in Math (1983)"
permalink: /apps/pcx86/1983/adventmath/
machines:
  - type: pcx86
    id: ibm5150
    config: /devices/pcx86/machine/5150/cga/64kb/machine.xml
    autoMount:
      B:
        path: /apps/pcx86/1983/adventmath/ADVENTMATH100.json
---

Adventures in Math (1983)
-------------------------

{% include machine.html id="ibm5150" %}

This game is available from the [Internet Archive](https://archive.org/details/msdos_Adventures_in_Math_1983).
The contents of their ZIP archive contains:

	-rwxr-xr-x@ 1 Jeff  staff  18688 Dec 24  1996 Adventur.bas
	-rwxr-xr-x@ 1 Jeff  staff      0 Dec 24  1996 Adventures in Math (1983).ba1
	-rwxr-xr-x@ 1 Jeff  staff  54277 Dec 24  1996 Basica.exe
	-rwxr-xr-x@ 1 Jeff  staff  11904 Dec 24  1996 Castle.bas
	-rwxr-xr-x@ 1 Jeff  staff   6400 Dec 24  1996 Exit.bas
	-rwxr-xr-x@ 1 Jeff  staff   4992 Dec 24  1996 Help.bas
	-rwxr-xr-x@ 1 Jeff  staff   1418 Dec 24  1996 Maze1
	-rwxr-xr-x@ 1 Jeff  staff   2179 Dec 24  1996 Maze2
	-rwxr-xr-x@ 1 Jeff  staff   3892 Dec 24  1996 Maze3
	-rwxr-xr-x@ 1 Jeff  staff  10496 Dec 24  1996 Monocode.000
	-rwxr-xr-x@ 1 Jeff  staff     15 Dec 24  1996 Run.bat
	-rwxr-xr-x@ 1 Jeff  staff     13 Dec 24  1996 Sn
	-rwxr-xr-x@ 1 Jeff  staff    369 Dec 24  1996 Topten

What's a little disturbing about the above archive is that all the files are dated "Dec 24 1996".
However, if you dig around a bit more on the Internet Archive, you discover that
[A Large Collection of DOS Collections](https://archive.org/details/large_dos_collection_2013_08) contains:

- DOS Collection v0.7/DVD1/Adventures In Math (1983)(Ibm).zip
- main torrent/1983/Adventures in Math (1983)(IBM) [Educational].zip

In the first ZIP file:

	-rw-r--r--@ 1 Jeff  staff  18688 Dec 24  1996 adventur.bas
	-rw-r--r--@ 1 Jeff  staff     16 Dec 24  1996 autoexec.bat
	-rw-r--r--@ 1 Jeff  staff  54277 Dec 24  1996 basica.exe
	-rw-r--r--@ 1 Jeff  staff  11904 Dec 24  1996 castle.bas
	-rw-r--r--@ 1 Jeff  staff   4964 Dec 24  1996 command.com
	-rw-r--r--@ 1 Jeff  staff   6400 Dec 24  1996 exit.bas
	-rw-r--r--@ 1 Jeff  staff   4992 Dec 24  1996 help.bas
	-rw-r--r--@ 1 Jeff  staff   1418 Dec 24  1996 maze1
	-rw-r--r--@ 1 Jeff  staff   2179 Dec 24  1996 maze2
	-rw-r--r--@ 1 Jeff  staff   3892 Dec 24  1996 maze3
	-rw-r--r--@ 1 Jeff  staff  10496 Dec 24  1996 monocode.000
	-rw-r--r--@ 1 Jeff  staff     13 Dec 24  1996 sn
	-rw-r--r--@ 1 Jeff  staff    369 Dec 24  1996 topten

And in the second ZIP file:

	-rw-r--r--@ 1 Jeff  staff  18688 Aug 11  1983 Adventur.bas
	-rw-r--r--@ 1 Jeff  staff  54277 Sep 17  1999 Basica.exe
	-rw-r--r--@ 1 Jeff  staff  11904 Aug 11  1983 Castle.bas
	-rw-r--r--@ 1 Jeff  staff   6400 Aug 11  1983 Exit.bas
	-rw-r--r--@ 1 Jeff  staff   4992 Aug 11  1983 Help.bas
	-rw-r--r--@ 1 Jeff  staff   1418 Aug 11  1983 Maze1
	-rw-r--r--@ 1 Jeff  staff   2179 Aug 11  1983 Maze2
	-rw-r--r--@ 1 Jeff  staff   3892 Aug 11  1983 Maze3
	-rw-r--r--@ 1 Jeff  staff  10496 Dec 19  1985 Monocode.000
	-rw-r--r--@ 1 Jeff  staff     15 Jan  4  2003 Run.bat
	-rw-r--r--@ 1 Jeff  staff     13 Aug 11  1983 Sn
	-rw-r--r--@ 1 Jeff  staff    369 Sep 17  1999 Topten
	-rw-r--r--@ 1 Jeff  staff    170 Jan 22  2011 file_id.diz

I decided to start with the contents of the second ZIP file.

One strange file common to *all* these archives is **MONOCODE.000**.  Dumping that file reveals:

	00000c60  20 4d 4f 4e 4f 50 4f 4c  59 20 69 73 20 61 20 72  | MONOPOLY is a r|
	00000c70  65 67 69 73 74 65 72 65  64 20 74 72 61 64 65 6d  |egistered tradem|
	00000c80  61 72 6b 20 6f 66 20 50  61 72 6b 65 72 20 42 72  |ark of Parker Br|
	00000c90  6f 74 68 65 72 73 2c 20  49 6e 63 2e e8 f7 7d e8  |others, Inc...}.|
	00000ca0  a1 64 e8 d4 79 e8 d6 7d  3c 20 20 20 20 20 20 20  |.d..y..}<       |
	00000cb0  20 20 20 20 20 20 4d 53  2d 44 4f 53 20 61 64 61  |      MS-DOS ada|
	00000cc0  70 74 61 74 69 6f 6e 20  28 43 29 20 31 39 38 35  |ptation (C) 1985|
	00000cd0  20 44 6f 6e 20 50 68 69  6c 6c 69 70 20 47 69 62  | Don Phillip Gib|
	00000ce0  73 6f 6e 20 5b e8 96 7d  03 35 2e 31 b8 5d 00 50  |son [..}.5.1.].P|

So at some point, unrelated ("MONOPOLY") files were mingled with this game.  I deleted the file.

Another unexpected file is **BASICA.EXE** (54277 bytes) from 1999.  It seems unlikely that IBM would have distributed
*any* BASIC binary with this game, because DOS was a prerequisite, and at the time, all versions of DOS included BASIC.
IBM's PC-DOS shipped with **BASICA.COM**, and OEM versions of DOS shipped with either **GWBASIC.EXE** or **BASIC.EXE**.

The closest matching binary I'd seen up to this point was **BASICA.EXE** from COMPAQ DOS 1.12 (54304 bytes).
And sure enough, examining the strings contained inside this **BASICA.EXE** revealed that it is a close relative:

	The COMPAQ Personal Computer BASIC
	Version 1.13
	(C) Copyright COMPAQ Computer Corp. 1983

It's safe to say that IBM would not have distributed a COMPAQ binary; if IBM had distributed any BASIC binary at all,
it would have been their own **BASICA.COM**.  Of course, the problem with IBM's **BASICA.COM** is that it also requires
an IBM PC with ROM BASIC installed, which is why someone copied the COMPAQ version of BASIC (it has no ROM dependencies).

Anyway, I've deleted **BASICA.EXE**.  The proper thing to do -- and what any purchaser of this game would have to do --
is boot a machine with an appropriate version of DOS and use the BASIC binary included with DOS to run this game.

Finally, there was **FILE_ID.DIZ**:

	Adventures in Math (1983)(IBM) [Educational].zip
	Name:Adventures in Math
	Version:1.0
	Language/Country:English
	Flags:
	Year:1983
	Publisher:IBM
	Genre(s):Educational

and **RUN.BAT**:

	basica castle

and **TOPTEN**:

	The Ultimate One,83519,LARGE,07-15-81
	MathsWhiz,78613,LARGE,01-01-80
	[z],70946,LARGE,07-13-81
	[z],56728,LARGE,04-24-80
	[z],56727,LARGE,07-25-81
	[z], 56277,LARGE,07-28-81
	[z],56157,LARGE,07-24-81
	[z],55677,LARGE,07-24-81
	[z],55197,LARGE,07-23-81
	[z],54792,LARGE,07-23-81
	^Z,07-28-81
	[z],56157,LARGE,07-24-81
	Z[z],55677,LARGE,07-24-81
	[z],55197,LARGE,07-23-81

All those files have been deleted as well, leaving 8 files dated "Aug 11 1983".  Next, I created a disk image from the
directory containing just those files:
 
	diskdump --dir=archive --format=json --output=ADVENTMATH100.json --manifest