# Plus4Serial
Plus4Serial is an Open Hardware Serial Port Adapter that plugs into the Commodore Plus/4 User Port, turning it into a fully-functional RS-232 interface.

![Board](https://raw.githubusercontent.com/SukkoPera/Plus4Serial/master/img/render-top.png)

## Summary
The +4 User Port has all the signals required by an RS-232 interface, but they are at TTL voltage levels (i.e.: 0/+5V). In order to turn them into a real RS-232 port, they need to be shifted to higher voltages, which is the purpose of this board.

All the signals available on the DB-9 port are translated and usable: RXD, TXD, RTS, CTS, DTR, DSR and DCD. The only exception is RI (Ring Indicator), which is left unconnected.

## Notes
This board uses a MAX238 chip for the level shifting, which is nice because it only needs a +5VDC voltage supply. The 9VAC supply available on the User Port is therefore not used. You can find used ones from China easily and cheaply.

If you are looking for a terminal emulator, I recommend [Term-80](https://plus4world.powweb.com/software/Term-80_English) as it is hands down the most feature-rich program of its kind (Hint: press <kbd>CBM+H</kbd> when you get lost) and supports communication at 19200 bps (Take that, C64!).

## License
The Plus4Serial documentation, including the design itself, is copyright &copy; SukkoPera 2022 and is licensed under the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/).

This documentation is distributed *as is* and WITHOUT ANY EXPRESS OR IMPLIED WARRANTIES whatsoever with respect to its functionality, operability or use, including, without limitation, any implied warranties OF MERCHANTABILITY, SATISFACTORY QUALITY, FITNESS FOR A PARTICULAR PURPOSE or infringement. We expressly disclaim any liability whatsoever for any direct, indirect, consequential, incidental or special damages, including, without limitation, lost revenues, lost profits, losses resulting from business interruption or loss of data, regardless of the form of action or legal theory under which the liability may be asserted, even if advised of the possibility or likelihood of such damages.

## Thanks
* TLC (Levente Hársfalvi) for lots of information about the serial port.
* The 3D model of the User Port connector was grabbed from [GrabCAD](https://grabcad.com/library/commodore-c64-userport-connector-1) but unfortunately the link now seems dead and I don't know who should be credited for it.

## Support the Project
You can buy me a coffee if you want:

<a href='https://ko-fi.com/L3L0U18L' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://az743702.vo.msecnd.net/cdn/kofi2.png?v=2' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>
