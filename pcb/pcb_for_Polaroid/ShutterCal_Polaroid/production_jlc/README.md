# JLCPCB assembly files — Polaroid calibrator rev 1.0

`BOM_JLC.csv` + `CPL_JLC.csv` for **Economic PCBA, bottom side**. Generate the gerbers from `../ShutterCal_Polaroid.kicad_pcb`: 2 layers, 1.6 mm, don't panelize.

- R4 = 6.8k (GND side) and R5 = 330k (+5V side) give ~0.10 V at the op-amp's + input. The schematic was fixed to match the routed copper.
- R6/R7 = 5.1k, the USB-C sink pull-downs on CC1 and CC2.
- R2 = 100k, a JLC basic part. The original was 91k, and the firmware only uses relative thresholds.
- Hand-fit: D1 (SFH 2440, LCSC C2900227) on the top side. J2 is the SWD header for flashing.
- The CPL rotations follow JLC's bottom-side convention, and were checked against JLC's footprint for every part.
