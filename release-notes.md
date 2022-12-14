---
title: What's new in Microsoft Defender for Firmware for device builders
description: Learn about the latest updates for Defender for Firmware for device builders.
ms.topic: conceptual
ms.date: 12/13/2022
---

# What's new

This article lists new features and feature enhancements in Microsoft Defender for Firmware for device builders.

Noted features are in **PREVIEW.** The [Azure Preview Supplemental Terms](https://azure.microsoft.com/support/legal/preview-supplemental-terms/) include other legal terms that apply to Azure features that are in beta, preview, or otherwise not yet released into general availability.

## Mid-December 2022

Most of the changes this month are behind the scenes in the architecture of our analysis pipeline -- we changed the underlying infrastructure hosting our services so that they are more secure and reliable, but that shouldn't change the results or add new analyzers.

### Added

- Allow users to modify selection of firmware while overview side panel is open

- Aria labels added to non-textual buttons to meet accessibility compliance

- Show the subscription name along with the subscription id in the firmware details panel

### Changed

- Refactored side panels to include footer buttons and fix various bugs (see below)

- Updated Portal SDK version to 10.204.0.1, and global .net core SDK to version 5.0.414

### Fixed

- Firmware analysis updates properly when clicking to select another firmware while overview panel is open

- Long firmware metadata strings are truncated properly in the overview panel now

- Firmware inventory doesn't lose its nerve and reset the view any more when user selects a different firmware row while overview panel is open

- The copy to clipboard icon in error boxes grew a backbone, no longer runs away when being hovered over

- Truncated path lists in analysis table columns are serious business now too and have stopped playing hide-and-seek when hovering over them at very specific page widths

- All overview panes with grey labels now meet color contrast accessibility guidelines

- Fix copy icon from inadvertently refreshing the inventory
