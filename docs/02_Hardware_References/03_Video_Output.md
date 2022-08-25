The Graphic controller of the **UDOO Vision** is the integrated **Intel&reg; HD Graphics 500**.  
Depending of the UDOO Vision version this are the specification:

* Intel&reg; HD Graphics 405 Up to 700 MHz 16 execution units (**ULTRA** version)
* Intel&reg; HD Graphics 400 Up to 640 MHz 12 execution units (**ADVANCED PLUS**)


### Decoding/Encoding specification

|             | formats                                       |
|-------------|-----------------------------------------------|
| HW decoding | HEVC(H.265), H.264, AVC, VC-1, VP8, VP9, JPEG |
| HW encoding | HEVC(H.265), H.264, VP8, AVC, JPEG            |


### Video Output Connectors

The Intel&reg; Atom&reg; Apollo Lake E3900 series of SoCs can support up to three independent 4K Ultra HD displays.

On the UDOO VISION board are exposed an **embedded Display Port** connector and a **Multimode Display Port** using a mini DP connector.

#### eDP Connector

On the boottom side of UDDO VISION is located the embedded Display Port connector.  
To use a display connected to this type of port, you need a connector type STARCONN p/n 300E30-0110RA-G3 or equivalent.

The maximum resolution available is 3840 x 2160 @60Hz.

#### miniDP++ Connector

On the UDOO VISION board, the Digital Display Interfaces #0 used to implement a multimode Display Port (DP++) interface,
i.e. it can be used to support DP displays directly and, through an external adapter, also HDMI or DVI displays.

The configuration of this interface in DP or HDMI/DVI mode is automatic.

The maximum available is 2560x1600 @ 60Hz.

You can use this [MiniDP++ to DP](http://shop.udoo.org/cable-minidp-to-dp.html) cable to connect to a DisplayPort display in 4k resolution.  
You can use this [MiniDP++ to HDMI](http://shop.udoo.org/cable-minidp-to-hdmi.html) cable to connect to an HDMI display in FullHD resolution. To have 4k resolution from mDP to HDMI you need an active adapter.



### UDOO Vision Hardware and UEFI BIOS User Manual

For a complete explanation of the UDOO Vision hardware you can download the [UDOO Vision Hardware and UEFI User Manual](https://udoo.org/download/files/UDOO_VISION/Doc/UDOO_VISION_MANUAL.pdf)
