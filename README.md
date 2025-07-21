# ForceY2K

ForceY2K is a very small system extension for Macintosh System 7. When the INIT code is run at boot, it sets the datetime in the Mac's clock chip to 1st Jan 2000.

It is intended for users who 1) don't use a PRAM battery in their old Macs and 2) may not be able to set the time over a network.

Solutions already previously existed for this problem, so I mainly did this as an exercise to learn what's involved in writing a system extension for Mac OS, and to better understand how to manipulate the datetime in Mac OS via code.

As the system thinks a valid datetime is set, it therefore won't display the "Your clock is not set to a correct date" warning alert dialog after system boot. One more annoyance gone!

This has been tested using System 7.1 in mini vMac on macOS 12.7 'Monterey' and on real hardware, a Macintosh Colour Classic running System 7.1.

A 68kMLA forum member generously tested it on System 6 and found that changing the filetype from scri to INIT was enough to get it working under System 6.

The source code is also provided; it can be built with CodeWarrior Pro 4.

## Acknowledgements

Many thanks to 68kMLA forum members Phipli and cheesestraws for suggesting the solution and treellama for suggesting an appropriate name for it. Extra thanks to cheesestraws because a portion of code in this extension was borrowed from the Force32 extension.