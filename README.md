vlc-trans-lua
=============

VLC Lua extension for translating subtitles in realtime via online translators.
The purpose of this extension is to enforce learning of foreign languages. 
Just watch movies in their original language with their subtitles,
 and get the translation on the fly when necessary.

Requirements
------------

The only supported format is SRT subtitle.
The subtitle file name should be the same as movie filename but with ".srt" extension. This is due to the lack of VLC API, sorry.
Internet connection.

![Alt text](https://sites.google.com/site/vlctranslua/_/rsrc/1343639212279/home/Screen%20shot%202012-07-30%20at%203.02.14%20PM.png)


Install
-------

Put the file in the VLC subdir /lua/extensions, by default:

* Windows (all users): %ProgramFiles%\VideoLAN\VLC\lua\extensions\
* Windows (current user): %APPDATA%\VLC\lua\extensions\
* Linux (all users): /usr/share/vlc/lua/extensions/
* Linux (current user): ~/.local/share/vlc/lua/extensions/
* Mac OS X (all users): /Applications/VLC.app/Contents/MacOS/share/lua/extensions/ 

Create directories if they don't exist.

Restart the VLC.

Enable the extension by going to the "View" menu and selecting it.


How to use
----------

When in pause press F12 to translate current subtitle.

![Alt text](https://sites.google.com/site/vlctranslua/_/rsrc/1343639234551/home/Screen%20shot%202012-07-30%20at%203.01.35%20PM.png)

Tweaking
--------
You can tweak some params in the beginning of the file:

Languages:

**SOURCE_LANG** = "en"  
**TARGET_LANG** = "ru"  

Translation engines: yandex, or google 

**translator** = "yandex" 

OSD:

**osd_duration** = 10
**osd_position** = "top-left"

