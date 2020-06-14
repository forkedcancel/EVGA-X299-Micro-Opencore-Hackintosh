# EVGA-X299-Micro-Opencore-Hackintosh
EFI folder for an X299 Hackintosh

GPU used is Sapphire RX 590 Nitro.

This configuration is now working. NVRAM works (Above 4G Encoding had to be disabled, contrary to opencore instructions). To fix the freezing, I used the OC wizard in the BIOS (I'm on 1.24) with the per core setting, and then dropped each core 200mhz below what it came up with, but I left the vcore settings it selected, which is the real reason I ran the wizard. I believe memory is set to 1.35V or 1.4V and XMP mode. It was the vcore changes that really made the machine stable, though.
