---
title: What is Microsoft Defender for Firmware for device builders?
description: Learn about how Microsoft Defender for Firmware helps device builders to market and deploy highly secure IoT/OT devices.
ms.topic: overview
ms.date: 11/10/2022
#Customer intent: As a device builder, I want to understand how Defender for Firmware can help secure my IoT/OT devices and products.
---

# What is Microsoft Defender for Firmware for device builders?

For IoT device builders, security is a near-universal concern. IoT devices have traditionally lacked basic security measures. But now with Microsoft Defender for Firmware, IoT device builders can quickly and easily identify embedded security threats and vulnerabilities that were previously undetectable.

Microsoft Defender for Firmware provides you the tools needed to deploy secure IoT firmware with:

- **Software Bill of Materials (SBOM)**: Receive a detailed listing of open-source packages used during the firmware's build process. In addition to the open-source packages used, you will see which version of the package is installed and what license governs the use of the open-source package.

- **CVE Analysis**: Quickly see which firmware components have publicly known security vulnerabilities and exposures.

- **Binary Hardening Analysis**: Identify binaries that have not enabled specific security flags during compilation like buffer overflow protection, position independent executables, and more common hardening techniques.

- **SSL Certificate Analysis**: Reveal expired and revoked SSL certificates.

- **Public & Private Key Analysis**: Verify the public and private cryptographic keys discovered in the firmware are necessary and not accidental.

- **Password Hash Extraction**: Ensure user account password hashes were created with secure cryptographic algorithms.  

## What is firmware?

Just like computers have operating systems, IoT devices have firmware. It's the firmware that runs and controls IoT devices.

## Why is firmware security important?

IoT attack vectors typically leverage easily exploitable--but easily correctable--weaknesses such as hardcoded user accounts, outdated and vulnerable open-source packages, or a manufacturer's private cryptographic signing key. By securing your IoT firmware against these common weaknesses, attackers will move on to a more vulnerable device.

## How can I be sure my firmware is secure?

Microsoft Defender for Firmware will analyze your firmware for these common weakness and vulnerabilities. As a device builder, you will have unparalleled insights into the security of your firmware whether you build the firmware ih-house, receive firmware from your supply chain, or engage in hybrid firmware development model (supply chain and in-house development).

## Next steps

[Analyze a firmware image.](quickstart-upload-firmware.md)

[Understand the firmware analysis results.](how-to-understand-firmware-results.md)
