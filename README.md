# Regain access to the BIOS of (almost) any ThinkPad
## Or, for that matter, any PC that uses an EEPROM to store a forgotten BIOS supervisor password

*_Disclaimer: This guide is intended for educational purposes only. The methods contained herein will most likely void the warranty of any system you attempt to compromise, and could potentially destroy your motherboard and / or any related hardware. Proceed with caution!_

### BIOS and Restricted Access
All modern PCs I know of allow for a few levels of restricted access that can be configured to take effect at boot time, most of which can be easily circumvented with a little tinkering.

![Power-On Password](https://github.com/zacacollier/no-more-thinkpad-super/blob/master/images/59377_poweronpwrd.gif?raw=true)

A common instance is a forgotten [*Power-On Password*](https://support.lenovo.com/us/en/documents/ht036206#power), which can be easily removed by opening up the computer and disconnecting a small *back-up battery* that's connected to the [CMOS](http://www.computerhope.com/issues/ch001360.htm), thereby voiding its contents - including the Power-On Password. Then you would power on your computer, enter the BIOS to reset your Date and Time settings (which were also removed from CMOS memory), and proceed to configure the BIOS.

There are similar methods for overriding the other forms of restricted access, such as a *hard drive password*, that can be easily found online. Regardless of the manufacturer, the basic concepts are usually the same.

### The Supervisor Password

For the highest level of BIOS password-protection - the Supervisor Password - there usually is no official solution - Lenovo, for instance, says _verbatim_: ["there is no way to reset"](https://support.lenovo.com/us/en/documents/ht036206#super) a forgotten Supervisor password. Your only option is to bring your proof of purchase to a certified Lenovo tech and pay to have the motherboard replaced.

You can imagine my disappointment when, after purchasing a very cheap "for-parts" t420s on Ebay, I discover that it not only has a Supervisor password set, but that there are no officially supported options provided by Lenovo - outside of replacing the motherboard entirely. Why, according to the manufacturer, is this not possible?

A little searching led me to discover that these generations of laptops stored the BIOS Supervisor Password on a tiny piece of hardware called an EEPROM - which curiously enough is defined as:
> ["a read-only memory whose contents can be erased and reprogrammed using a pulsed voltage."](https://www.google.com/webhp?sourceid=chrome-instant&ion=1&espv=2&ie=UTF-8#q=what+is+an+eeprom)


