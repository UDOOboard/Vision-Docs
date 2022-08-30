### eMMC onboard

Depending on the [chosen model](!Hardware_References/Board_versions) of UDOO VISION, your board may be equipped with an eMMC storage memory up to 64GB to install your favorite OS.  

The eMMC use a **SD 3.0** compliant interface.

<span class="label label-warning">Heads up!</span> As a flash-based storage device, excessive drive access, particularly write commands, reduces its useful life. Therefore, it is strongly suggested to NOT create a swap partition on the eMMC device.


### S-ATA

Both Apollo Lake E3940 and E3950 processors embed a SATA Controller, which offers up to two **SATA III 6.0 Gbps** interfaces.  
Of these interfaces, one SATA channel is carried out to a standard male S-ATA connector, CN11 (the other SATA channel is available on the M.2 Key B socket).

A dedicated power connector (*CN10*), can be used to power *2.5"* Hard Disk Drives (or Solid State Drives) connected to the SATA male connector.  
The dedicated power connector is a 4-pin male connector. You can find this cable in the [SATA data and power cables for UDOO Vision](https://shop.udoo.org/en/catalogsearch/result/?q=+Sata++data+and+power+cables) kit.

<span class="label label-warning">Heads up!</span> To connect a *3.5"* Hard Drive you need to provide SATA +5V+12V combo power supply from an external source.

### μSD

The SoCs used on UDOO VISION module offer a **SD/MMC 4.0** compliant interface, that can be used as a boot device and/or to implement another mass storages media other than the optional internal eMMC and the two SATA interfaces.
This SD interface is carried to a standard μSD card slot (*CN13*), soldered on bottom side of the module, push-push type.

### M.2 SATA Slot: Socket 2 Key B type 3042/2260

The mass storage capabilities of the UDOO VISION are completed by an M.2 SSD Slot, which allow plugging **M.2 Socket 2 Key B** Solid State Drives with *SATA* interface.  

The connector used for the M.2 SATA slot is *CN14*, which is a standard 75 pin M.2 Key B connector.

On the UDOO VISION board there is also a Threaded Spacer which allows the placement of M.2 Socket 2 Key B SATA/PCI-e modules in `2260` or `3042` sizes.

For the additional informations about M.2 connectors, look at the [relative section](Hardware_References/M.2_Connectors).