# IoT Firmware Customization Dataset

This dataset accompanies our study of firmware update strategies among Linux-based IoT devices, focusing specifically on update customization—a widely overlooked yet security- and efficiency-critical aspect.

## 📚 Motivation

Various defense strategies have been proposed to secure the firmware update process, but **update customization** remains a **pitfall** for both security and efficiency. Unlike general protection mechanisms such as signature verification or rollback prevention, customization in updates—whether manufacturer-driven or user-defined—has received scant attention from the research community.

To explore this gap, we conducted a **pilot study** on the firmware update mechanisms of over **200 Linux-based IoT devices**, including routers, smart home devices, and sensors, spanning **23 different vendors**.

## 🔍 Research Scope

Due to the lack of standardized guidelines, manufacturers vary greatly in how they implement and support customization. For example:

- **OpenWrt** typically releases firmware components on a central server, requiring users to manually install updates.
- **Netgear**, in contrast, integrates automatic update services that push updates to devices directly upon release.

To better understand the **security implications** of such strategies, we:

1. Conducted empirical analyses on manufacturers' firmware customization practices.
2. Reviewed over 200 firmware instances from both **open-source** and **commercial** vendors.
3. Developed an evaluation framework based on four key indicators:
   - Prevention of firmware rollback
   - Support for automatic updates
   - Update frequency
   - Package manager availability

## 📊 Dataset Overview

This repository provides a structured collection of firmware-related data from 23 vendors. For each vendor, we include:

- Device models and types
- Firmware sources (or links, if public)
- Notes on automatic update support, customization practices, and other metadata

Where licensing or ethical restrictions apply (e.g., Fortinet, Cisco), only device metadata is provided.

You can explore the full vendor dataset under their respective subdirectories, each accompanied by a `README.md` detailing:

- The number of supported models
- Device types
- Firmware download links (if publicly accessible)
- Observations from update strategy analysis

A summary of selected vendor strategies is presented below:

| Classification | Vendor  | Prevent Rollback | Automatic Update | Update Frequency | Package Manager |
|----------------|---------|------------------|------------------|------------------|-----------------|
| Open Source    | OpenWrt | ❌ No            | ❌ No            | ✅ Monthly       | ✅ opkg          |
|                | Tomato  | ❌ No            | ❌ No            | ❌ 6–12 months   | ❌ No            |
| Commercial     | Cisco   | ✅ Yes           | ✅ Yes           | ✅ Monthly       | ❌ No            |
|                | TP-Link | ✅ Yes           | ✅ Yes           | ⚠️ 3–6 months   | ❌ No            |
|                | Huawei  | ✅ Yes           | ✅ Yes           | ✅ Monthly       | ❌ No            |

## 🧩 Key Findings

- Open-source firmware (e.g., OpenWrt) prioritizes **flexibility and user customization** but often lacks security guarantees like rollback protection or automated updates.
- Commercial firmware (e.g., Cisco, Huawei, TP-Link) emphasizes **security and manageability**, frequently at the cost of **user customization capabilities**.
- Firmware update customization remains underdeveloped in both communities, limiting efficient adaptation to dynamic environments or specific user needs.

## 🔗 Reference

Part of this dataset is derived from the publicly available collection provided by:

> Wu, Yuhao, et al. "Your Firmware Has Arrived: A Study of Firmware Update Vulnerabilities."  
> *33rd USENIX Security Symposium (USENIX Security 24), 2024.*  
> [GitHub Dataset Repository](https://github.com/WUSTL-CSPL/Firmware-Dataset)

```bibtex
@inproceedings{wu2024your,
  title={Your Firmware Has Arrived: A Study of Firmware Update Vulnerabilities},
  author={Wu, Yuhao and Wang, Jinwen and Wang, Yujie and Zhai, Shixuan and Li, Zihan and He, Yi and Sun, Kun and Li, Qi and Zhang, Ning},
  booktitle={33rd USENIX Security Symposium (USENIX Security 24)},
  pages={5627--5644},
  year={2024}
}
