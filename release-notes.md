---
title: What's new in Microsoft Defender for Firmware for device builders
description: Learn about the latest updates for Defender for Firmware for device builders.
ms.topic: conceptual
ms.date: 11/18/2022
---

# What's new

This article lists new features and feature enhancements in Microsoft Defender for Firmware for device builders.

Noted features are in **PREVIEW.** The [Azure Preview Supplemental Terms](https://azure.microsoft.com/support/legal/preview-supplemental-terms/) include other legal terms that apply to Azure features that are in beta, preview, or otherwise not yet released into general availability.

## Mid-December 2022

Most of the changes this month are behind the scenes in the architecture of our analysis pipeline -- we changed the underlying infrastructure hosting our services so that they are more secure and reliable, but that shouldn't change the results or add new analyzers.

Additionally there are some tweaks in the UI as follows:

- New upload panel

- New firmware overview panel

- New firmware edit panel

- Fix bug where analysis details were not updating when user selects a different row

- Fix bug where firmware table was refreshing and moving scroll to top when user selects a different row

- Fix bug where long vendor/model/version strings were overflowing their grid and stomping all over each other

- Allow file input text width (name of file chosen on upload) to fill up width of panel
