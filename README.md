# DIY-UPS-for-WiFi-Router
A UPS for Wi-Fi routers and ONU with 4 hours of back-up.

# SPECIFICATIONS:
Here is a breif table containing the main specs of the UPS:
| CATEGORY | VALUE |
| :---: | :---: | 
| Back-UP time | Upto 4 hours|
| No. of Output ports | 2 |
| Output Voltage | 12V(1A) & 9V(800mA) |
| Input Voltage | 12V |
| Battery Type | 2s-2p li-ion |
| Battery Voltage | 7.4V(nominal) |
| Battery Capacity | 4000mAH |

# BATTERY PACK
The battery is a 2s 2p lithium-ion pack with a nominal voltage of 7.4 volts and a capacity of, 4000mAh approximately.
The batteries are managed by this HW-882 3 A BMS for 2s lithium-ion battery pack.

# POWER & CHARGING

## POWER:
Unlike many commercial devices, this DIY UPS utilises 2 * 12 volt adapter. One for powering the Router and ONU while the other charges the batteries.
The adapter connected to the female barrel port labelled ```12V-IN-MAIN``` power both the router and ONU, while the one connected to the female barrel port labelled ```12-IN-2ND``` is used for the charging the battery.
However, using two adapters is not a must, the entire thing can be powered by a single 12 volt adapter. To do so follow these steps:
- Short the pads ```TP1``` & ```TP2``` on the bottomside of the PCB.
- Now, plug the 12V adapter to the female barrel port labelled ```12V-IN-2ND```.

### Note:
 When using a single 12V adpater to power as well as charge the batteries, do not plug the 12V adapter into the female barrel port labelled ```12V-IN-MAIN```. Use the port labelled ```12V-IN-2ND```. Also use an adapter rated at-least 1.5 amps.
 
## CHARGING SYSTEM:
The batteries are charged by this XL4015 CC/CV 5A buck converter module, whose voltage and current must be set to 8.35 volts and 1.4 amps respectively.
The XL4015 module is powered by a 12V 2A adapter. If your 12V adapter is rated below 2A then lower the charging current on the buck converter to an appropriate level. Below are some reccommended charging current values in relation to the adapter's current rating:

| Adapter's Current Rating(A) | Charging Current(A) |
| :---: | :---: |
| 1 | 0.7 - 0.8 |
| 1.5 | 1 - 1.2 |
| 2 | 1.2 - 1.6 |
