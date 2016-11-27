# Regain access to the BIOS of (almost) any ThinkPad
#### _"Or, for that matter, any PC that uses an EEPROM to store administrative BIOS settings"_

*_Disclaimer: This guide is intended for educational purposes only. The methods contained herein will most likely void the warranty of any system hardware you attempt to compromise, and could potentially destroy your motherboard and / or any related hardware. Proceed with caution!_

## Introduction:

### BIOS and Restricted Access
All modern PCs I know of allow for a few levels of restricted access that can be configured to take effect at boot time. In the event that you find yourself unable to gain access, most of these restrictions can be easily circumvented with minimal effort.

![Power-On Password](https://github.com/zacacollier/no-more-thinkpad-super/blob/master/images/59377_poweronpwrd.gif?raw=true)

A common instance is a forgotten [*Power-On Password*](https://support.lenovo.com/us/en/documents/ht036206#power), which can be easily removed by opening up the computer and disconnecting a small *back-up battery* that's connected to the [CMOS](http://www.computerhope.com/issues/ch001360.htm), thereby voiding its contents - including the Power-On Password. Then you would power on your computer, enter the BIOS to reset your Date and Time settings (which have *also* been removed from CMOS memory), and proceed to configure the BIOS.

Similar methods for overriding other forms of restricted access such as a *hard drive password* can be easily obtained online; for most modern hardware architecture, these methods are (to my knowledge) conceptually the same - regardless of the manufacturer.

### The Supervisor Password

To bypass the highest level of BIOS password-protection - the Supervisor Password - there is most often *no official solution*. In my case, Lenovo's support documentation, for instance, says _verbatim_: ["there is no way to reset"](https://support.lenovo.com/us/en/documents/ht036206#super) a forgotten Supervisor password. Your _only option_ is to present a valid proof of purchase to a certified Lenovo tech and pay to have the motherboard replaced.

You can imagine my disappointment when, after purchasing a very cheap "for-parts" ThinkPad t420s on Ebay, I discover that it has a Supervisor password set, and find no support options from Lenovo other than an expensive motherboard replacement. This drastically discounted system, in excellent cosmetic condition, replete with a solid 2nd-gen i5 CPU, 6GB of RAM, as well as some compelling bells and whistles such as WiMax and mSATA compatability, was - in Lenovo's eyes - a *lemon*.

### A Brief Aside: Motivation

If you've read this far, you may have inferred that I _did_ find a solution, albeit an *unofficial* one. Obviously I wouldn't be writing this guide if I hadn't - in fact I'm doing so in part as a way to constructively (debatable?) kill time while the system in question compiles a fresh Gentoo installation.

Another reason is that for all my googling I have yet to find a single, go-to resource describing this technique; this is an attempt to rectify that.

Finally, I am writing this guide as a reflection of personal ethics. I understand where Lenovo, Dell, Apple, HP et al. are coming from - in business strategy there's almost always a more profitability in coercing your customers into buying replacement hardware rather than encouraging self-repair.

At best, I'm guessing that a confiscated motherboard will go sit in a repair queue somewhere. Another more probable (read: economically feasible) option is that the manufacturer - Lenovo in this case - will simply throw it away. It's a shame to see good hardware go to waste - especially beyond the immediately obvious anti-utilitarian consequences. E-waste is a *rapidly-growing ecological and humanitarian concern* that has a [profound impact](http://www.techrepublic.com/article/the-depressing-truth-about-e-waste-10-things-to-know/) on the well-being of the developing nations where it accumulates.

Nowadays there are many formidably large-scale efforts aiming to address E-waste management, and more and morecomputer hardware manufacturers are becoming active participants. Nevertheless, as a consumer of electronics, it's good to stay informed on what you can do to better manage your *individual* level of impact. Breathing life into an otherwise inaccessible PC is a very rewarding way to do just that, and it has the added bonus of being a very inexpensive way to add another system to your collection.

#### Who's this guide for, then?
This is great for anyone looking for a project PC, something you're not afraid to tinker with and possibly break. I, for instance, was looking for a cheap laptop I could use for learning more about Linux.

If you're in the market for a daily driver, that is, you're looking to purchase a system that *you intend to be your primary workstation*, I don't recommend you invest the time and effort in this method. Consider a used or refurbished system (craigslist is always a good resource). Read up on manufacturer warranties and how you might acquire one for a secondhand system - Applecare, for instance, can be purchased for a system up to one year after it's date of initial purchase, [regardless of prior ownership](https://discussions.apple.com/thread/5249998?start=0&tstart=0). 


