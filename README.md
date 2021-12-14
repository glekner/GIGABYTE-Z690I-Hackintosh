# Z690I Aorus OpenCore EFI

EFI Partition and Guidelines for my Mini-ITX Hackintosh

![About](./assets/about.png)

## Hardware

- Phanteks Evolv Shift 2 Air
- Gigabyte Z690I Aorus
- Intel Core i7-12700K
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

## ACPI

1. SSDT-PLUG-ALT.aml
2. SSDT-GPRW.aml - _GPRW is required for reliable sleep, wake is only triggered by power button_
3. SSDT-AWAC-DISABLE.aml
4. SSDT-EC-USBX.aml
5. SSDT-DMAC.aml
6. SSDT-DTPG.aml

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
