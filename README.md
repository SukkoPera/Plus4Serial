# Plus4Serial
Plus4Serial is an Open Hardware Serial Port Adapter that plugs into the Commodore Plus/4 User Port, turning it into a fully-functional [RS-232 interface](https://en.wikipedia.org/wiki/RS-232).

![Board](https://raw.githubusercontent.com/SukkoPera/Plus4Serial/master/img/render-top.png)

## Summary
The Plus/4 User Port has all the signals required by an RS-232 interface, but they are at TTL voltage levels (i.e.: 0/+5V). In order to turn them into a real RS-232 port, they need to be shifted to higher voltages, which is the purpose of this board.

All the signals available on the DE-9 port are translated and usable: RXD, TXD, RTS, CTS, DTR, DSR and DCD. The only exception is RI (Ring Indicator), which is left unconnected.

The board plugs in the User Port, which means that it can also be used on a C16 or C116 through [a User Port card](https://github.com/SukkoPera/16up).

## Notes
This board uses a MAX238 chip for the level shifting, which is nice because it only needs a +5VDC voltage supply. The 9VAC supply available on the User Port is therefore not used. You can find used ones from China easily and cheaply.

If you have an older version of the board with a CTS/_CTS jumper, place it in the _CTS position, as it's the only correct one.

If you are looking for a terminal emulator, I recommend [Term-80](https://plus4world.powweb.com/software/Term-80_English) as it is hands down the most feature-rich program of its kind (Hint: press <kbd>CBM+H</kbd> when you get lost) and supports communication at 19200 bps (Take that, C64!).

## Releases
If you want to get this board produced, you are recommended to get [the latest release](https://github.com/SukkoPera/Plus4Serial/releases) rather than the current git version, as the latter might be under development and is not guaranteed to be working.

Every release is accompanied by its Bill Of Materials (BOM) file and any relevant notes about it, which you are recommended to read carefully.

## License
The Plus4Serial documentation, including the design itself, is copyright &copy; SukkoPera 2022 and is licensed under the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/).

This documentation is distributed *as is* and WITHOUT ANY EXPRESS OR IMPLIED WARRANTIES whatsoever with respect to its functionality, operability or use, including, without limitation, any implied warranties OF MERCHANTABILITY, SATISFACTORY QUALITY, FITNESS FOR A PARTICULAR PURPOSE or infringement. We expressly disclaim any liability whatsoever for any direct, indirect, consequential, incidental or special damages, including, without limitation, lost revenues, lost profits, losses resulting from business interruption or loss of data, regardless of the form of action or legal theory under which the liability may be asserted, even if advised of the possibility or likelihood of such damages.

## Support the Project
If you want to get some boards manufactured, you can get them from PCBWay through this link:

[![PCB from PCBWay](https://www.pcbway.com/project/img/images/frompcbway.png)](https://www.pcbway.com/project/shareproject/TBD)

You get my gratitude and cheap, professionally-made and good quality PCBs, I get some credit that will help with this and [other projects](https://www.pcbway.com/project/member/shareproject/?bmbid=41100). You won't even have to worry about the various PCB options, it's all pre-configured for you!

Also, if you still have to register, [you can use this link](https://www.pcbway.com/setinvite.aspx?inviteid=41100) to get some bonus initial credit (and yield me some more).

You can also buy me a coffee if you want:

<a href='https://ko-fi.com/L3L0U18L' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://az743702.vo.msecnd.net/cdn/kofi2.png?v=2' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>

## Thanks
* TLC (Levente Hársfalvi) for lots of information about the serial port.
* The 3D model of the User Port connector was grabbed from [GrabCAD](https://grabcad.com/library/commodore-c64-userport-connector-1) but unfortunately the link now seems dead and I don't know who should be credited for it.
