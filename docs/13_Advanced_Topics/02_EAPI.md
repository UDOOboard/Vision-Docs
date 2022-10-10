EAPI (Embedded Application Programming Interface) is a framework
developed by *PICMG®* for *COM Express* modules that gives a common API to unify
software control for:
- System information
- Watchdog timer
- I2C Bus
- Flat Panel brightness control
- User storage area
- GPIO

The EAPI definition is open to be used for other embedded form factors too,
such as SBCs. Read the full specification [here][https://www.picmg.org/wp-content/uploads/COM_EAPI_R1_0.pdf].

The EAPI implementation for UDOO VISION can be found [here](https://git.seco.com/software/eapi/eapi/-/tree/master/binary) for both
Windows and Linux.  
As you can see [here](https://git.seco.com/software/eapi/eapi/-/wikis/home#seco-implementation), the UDOO VISION doesn't have
an official version by now but we are working to provide you a stable and tested release.