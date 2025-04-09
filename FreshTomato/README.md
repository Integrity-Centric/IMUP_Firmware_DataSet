# FreshTomato Firmware Dataset

This directory contains firmware download information for **FreshTomato**, an enhanced Tomato firmware fork supporting Broadcom-based routers.

## 🔢 Dataset Overview

- **Number of Devices**: 10
- **Device Types**: Routers (ARM & ARMv7-based)

## 🌐 Firmware Download Links

| Device Model      | Firmware Version | Firmware Type | Download Link |
|-------------------|------------------|----------------|---------------|
| Linksys EA6200    | 2022.1           | AIO-64K         | [Download](https://freshtomato.org/downloads/freshtomato-arm/2022/2022.1/K26ARM/freshtomato-EA6200-ARM_NG-2022.1-AIO-64K-NOSMP.zip) |
| Linksys EA6350v2  | 2022.1           | AIO-64K         | [Download](https://freshtomato.org/downloads/freshtomato-arm/2022/2022.1/K26ARM/freshtomato-EA6350v2-ARM_NG-2022.1-AIO-64K.zip) |
| Linksys EA6400    | 2022.1           | AIO-64K         | [Download](https://freshtomato.org/downloads/freshtomato-arm/2022/2022.1/K26ARM/freshtomato-EA6400-ARM_NG-2022.1-AIO-64K.zip) |
| Netgear R6250     | 2022.1           | AIO-64K         | [Download](https://freshtomato.org/downloads/freshtomato-arm/2022/2022.1/K26ARM/freshtomato-R6250-ARM_NG-2022.1-AIO-64K.zip) |
| Netgear R7000     | 2022.1           | AIO-64K         | [Download](https://freshtomato.org/downloads/freshtomato-arm/2022/2022.1/K26ARM/freshtomato-R7000-ARM_NG-2022.1-AIO-64K.zip) |
| Netgear R8000     | 2022.3           | AIO-64K         | [Download](https://freshtomato.org/downloads/freshtomato-arm/2022/2022.3/K26ARM7/freshtomato-R8000-ARM-2022.3-AIO-64K.zip) |
| Netgear R8000     | 2022.3           | VPN-64K         | [Download](https://freshtomato.org/downloads/freshtomato-arm/2022/2022.3/K26ARM7/freshtomato-R8000-ARM-2022.3-VPN-64K.zip) |
| Asus RT-AC3200    | 2022.3           | AIO-128K        | [Download](https://freshtomato.org/downloads/freshtomato-arm/2022/2022.3/K26ARM7/freshtomato-RT-AC3200-ARM-2022.3-AIO-128K.zip) |
| Asus RT-AC3200    | 2022.3           | VPN-128K        | [Download](https://freshtomato.org/downloads/freshtomato-arm/2022/2022.3/K26ARM7/freshtomato-RT-AC3200-ARM-2022.3-VPN-128K.zip) |
| ARMv7 Utilities   | 2022.3           | extras          | [Download](https://freshtomato.org/downloads/freshtomato-arm/2022/2022.3/K26ARM7/extras-arm7.tar.gz) |

> ⚠️ **Note**: These firmware files are sourced from the official FreshTomato website. Ensure model and NVRAM compatibility before flashing.

## 📝 Notes

- FreshTomato is an open-source firmware based on Tomato, supporting modern Broadcom routers.
- Versions are divided by architecture (K26ARM / K26ARM7), firmware type (AIO / VPN), and NVRAM size (64K / 128K).
- AIO (All-in-One) includes all major modules; VPN builds are lighter with VPN tools.
- Visit [https://freshtomato.org](https://freshtomato.org) for changelogs and documentation.
- Verify firmware integrity using available `MD5SUM` files.
