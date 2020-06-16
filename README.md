# EVGA-X299-Micro-Opencore-Hackintosh
EFI folder for an X299 Hackintosh

GPU used is Sapphire RX 5600 XT Pulse. Fenvi card used for wifi and bluetooth (USBMap.kext has HS05 set to internal).

Originally I was using an RX 590 Pulse but ran into problems with hardware encoding/decoding which made the machine crawl to near unusable levels.

This configuration is now working. NVRAM works (Above 4G Encoding had to be disabled, contrary to opencore instructions). To fix the freezing, I used the OC wizard in the BIOS (I'm on 1.24) with the per core setting - the real reason for doing this is raising the voltages. You don't need to OC, you can just set voltage manually. The AUTO setting sets vcore to below 1V and this is why it freezes. If you also have a 7940X, maybe try 1.05V or 1.1V. I believe memory is set to 1.4V (stock for my RAM is 1.35V) and XMP mode. It was the vcore changes that really made the machine stable, though.
