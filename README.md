# Regain access to the BIOS of (almost) any ThinkPad
## Or, for that matter, any PC that uses an EEPROM to store a forgotten BIOS supervisor password

All modern PCs I know of allow for a few levels of protected access that can be set at boot time, many of which are easily circumvented with a little tinkering.

![Power-On Password](https://github.com/zacacollier/no-more-thinkpad-super/blob/master/images/59377_poweronpwrd.gif?raw=true)
For example, a forgotten [Power-On Password](https://support.lenovo.com/us/en/documents/ht036206#power) can be easily removed by opening up the computer and disconnecting a small *back-up battery* that's connected to the [CMOS](http://www.computerhope.com/issues/ch001360.htm), thereby voiding its contents, including the Power-On Password. You would then power on your computer and enter the BIOS to reset your Date and Time settings, which were also removed from CMOS memory.
