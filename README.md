# EVGA-X299-Micro-Opencore-Hackintosh

### Notice:
This repo is no longer maintained. I have replaced this machine with an M1 Mac Mini. It has fewer cores and inferior graphics performance compared to the hackintosh this EFI folder is for, but I'm tired of having to update this configuration periodically to stay up to date, and an i9-7940X will always run much hotter (and therefore louder) than the new Mini. My office is dead silent now. Even when all 8 cores are pegged during a compilie.

I hope this repo has been of use to others trying to make this hardware work with macOS.

## EFI folder for an EVGA X299 Micro Hackintosh

Note: My EVGA X299 Micro was the first revision, not the second. This may or may not matter.

GPU used is Sapphire RX 5600 XT Pulse. Fenvi card used for wifi and bluetooth (USBMap.kext has HS05 set to internal).

Originally I was using an RX 590 Pulse but ran into problems with hardware encoding/decoding which made the machine crawl to near unusable levels.

This configuration is now working. NVRAM works (Above 4G Encoding had to be disabled, contrary to opencore instructions). To fix the freezing, I used the OC wizard in the BIOS (I'm on 1.24) with the per core setting - the real reason for doing this is raising the voltages. You don't need to OC, you can just set voltage manually. The AUTO setting sets vcore to below 1V and this is why it freezes. If you also have a 7940X, maybe try 1.05V or 1.1V. I believe memory is set to 1.4V (stock for my RAM is 1.35V) and XMP mode. It was the vcore changes that really made the machine stable, though.
