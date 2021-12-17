# Z690I Aorus OpenCore EFI

EFI Partition and Guidelines for my Mini-ITX Hackintosh

![About](./assets/about.png)

## Changelog

```
0.0.2 - replaced all <integer>3</integer> with <integer>255</integer>
inside USBPorts.kext for USB3. this change fixes insta-wake,
therefore we can delete GPRW patches

0.0.1 - iniitial release
```

## Hardware

- Phanteks Evolv Shift 2 Air
- Gigabyte Z690I Aorus
- Intel Core i7-12700K
- EK-AIO 120 D-RGB
- G.Skill TridentZ RGB 2x16GB DDR4-3200CL14
- Gigabyte RX 6600XT 8GB OC
- LinkUP PCI-E 4.0 Riser
- 2xWD Black SN850 1TB NVMe
- Corsair SF500W
- BCM94352Z WiFi/BT

## Config

- SMBIOS - MacPro7,1
- Verbose Off
- Scaled for 4K
- `agdpmod=pikera` is enabled because i'm using an AMD GPU
- `AudioDxe.efi` is disabled by default for faster boot time

## Bios

Disabled:

- CFG-Lock
- Fast Boot
- VT-d
- CSM

Enabled:

- VT-x
- Above 4G decoding
- Re-Size BAR Support
- XHCI Hand-off

## Overclocking

- VCore: Fixed 1.28V
- DVID: -0.045
- LLC: 3
- P 0-1: 50
- P 2-7: 49
- E 0-3: 39

---

![Geekbench](./assets/geekbench.png)

![Case](./assets/case.JPG)
