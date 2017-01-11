# Generic "PC Remote" support for HTPC software

## Huh?

This is support for RasPlex or its cousins for USB remote controls that look
like this:

![Remote
control](https://raw.githubusercontent.com/davidjb/plex-usb-pc-remote/master/remote.jpg)

They can be had for around $5 AUD on
[eBay](www.ebay.com.au/itm/Remote-Infrared-Ray-Control-Controller-Wireless-PC-USB-Windows-Media-Center-/381210067916)
and other disreputable marketplaces.

## Install

The `pc-remote.xml` file should be installed on RasPlex in this
location:

    /storage/.plexht/userdata/keymaps/pc-remote.xml

You'll have to adjust the path for use with Kodi / XBMC and so on.  Also, the
file can actually be named `anything.xml`, providing it is in that directory.

## Use with a Logitech remote

The Logitech Remote control was customised to send different signals and
"hijack" other types of buttons to perform specialist actions.  For example,
the `My PC` button sends `0; e` keys so we map that to simply the `e` key to
open the `ContextMenu` in Plex. Within the Logitech Remote software we normalise
this so the `Menu` Logitech button sends the `My PC` button IR signal.

The `keypress-logs.txt` file contains a history of what every button on the
remote translates to and the `named_remote.txt` is a full record of the
default Plex keyboard configuration for a Media Centre remote.

## More info

* <https://github.com/RasPlex/RasPlex/wiki/Remote-Controls>
* <http://kodi.wiki/view/HOW-TO:Modify_keyboard.xml#Where_to_find_keyboard.xml>

