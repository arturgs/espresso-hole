# ESPRESSO-hole: ESPRESSObin based personal router with ad blocking.

This project was born as a solution to a set of requirements for a home box/router.

Hardware wish-list:
- gigabit router
- several (>2) ethernet ports
- external disk storage for server/media
- linux supported
- some USB ports

Network wish list:
- ad blocker, pi-hole style
- traffic redirected through VPN
- WIFI access point
- media server

The [Marvell ESPRESSObin](http://espressobin.net) fits all these hardware requirements at the reduced price of [$49](https://www.globalscaletechnologies.com/p-72-marvell-espressobin.aspx).

![Alt text](images/MotherBoard_1.png)

## Hardware setup



### External disk
The ESPRESSObin supports an external drive through a SATA connector. However, in v5 of the board (v7 is available now) the power connector is a molex-type connector. An adaptor to SATA power can be easily done, but minor soldering habilities are required.
![](images/sata_power.jpg)

### USB wireless

For wireless connection a USB WiFi dongle based on RT5370. Notice that not any dongle will work, or will be able to be set in AP mode.

### 3d printed case
The ESPRESSObin comes without a case. A number of slutions are available, I specially like [this one](https://upon2020.com/blog/2017/12/3d-printable-box-for-the-espressobin-plus-a-hard-disk/). The [STL file](https://www.thingiverse.com/thing:2707086) provided includes the two parts together, so I provide an [STL folder](http://github.com/arturgs/espresso-hole/tree/master/case_3d_print) with two separated parts.

The case is designed with room for a 25mm fan like [this one](https://www.banggood.com/Hobbywing-5V-7V-150A-DC-Cooling-Fan-For-RC-Model-Motor-ESC-253040mm-Power-Transfer-p-1067266.html?rmmds=myorder&ID=47301&cur_warehouse=CN). On normal operation I find the fan too noisy and temperature levels have never been dangerous without the fan.

## Armbian installation
The ESPRESSObin is fully supported by [ARMBIAN](https://docs.armbian.com). Installation can be done easily [as explained here](https://www.armbian.com/espressobin/).

## Network configuration
- VPN
- DNS
- DHCP
- wireless AP

### PI-HOLE installation


### HostApd service

## Additional Software 
