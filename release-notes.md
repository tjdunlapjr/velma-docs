---
title: What's new in Microsoft Defender for Firmware for device builders
description: Learn about the latest updates for Defender for Firmware for device builders.
ms.topic: conceptual
ms.date: 11/18/2022
---

# What's new

This article lists new features and feature enhancements in Microsoft Defender for Firmware for device builders.

Noted features are in **PREVIEW.** The [Azure Preview Supplemental Terms](https://azure.microsoft.com/support/legal/preview-supplemental-terms/) include other legal terms that apply to Azure features that are in beta, preview, or otherwise not yet released into general availability.

## Mid-November 2022

New Features and User-Facing Changes 

- Added new Binary Hardening analyzer, which shows whether executables in the firmware were built using recommended security settings 

- Added a brand new version of Binwalk Pro firmware extractor which is used to extract file systems from the firmware image; see below for details on supported file types 

- Improved support for analyzing large firmware images – previously they might get stuck in the “analyzing” state 

- Added support for single CVSS score in CVE results which is one of either the v3 score (preferred) or the v2 score 

- Older reports that don’t contain the single CVSS score and version will still show the 2 individual scores 

- Firmware delete dialog no longer greys out part of the frame in the background so it looks more natural 

- Allow user to click on table rows when detail side panels are open 

- Implement copy-to-clipboard button for certain values like firmware id and error correlation id 

- Show convenient human readable values for certain statistics like firmware size and file count 

- Rename Vulnerabilities tab to Weaknesses to match M365 Defender 

Notes 

- Currently the maximum size of a firmware image that can be uploaded in 1GB 

- The new Binwalk extractor does not yet support all the same file formats as the legacy Binwalk Enterprise solution – you will see different counts for files extracted and software components if your firmware image uses formats that are not yet supported. The following table shows which formats are supported: 

These formats are fully supported by the new Binwalk extractor: 


| File Format | Description
| ----------- | -----------
|  Gzip       | Gzip file compression
|  XZ         | XZ compression
|  BZ2        | BZip2 compression
|  LZ4        | LZ4 compression
|  TAR        | Tarball archive format
|  CPIO       | ASCII CPIO archive format
|  ZIP        | ZIP archive format
|  SquashFSv4 | SquashFS version 4 file system
|  CramFS     | CramFS file system (zlib & LZMA)
|  JFFS2      | JFFS2 file system
|  YAFFS      | YAFFS file system
|  UBIFS      | UBI file system
|  GPG        | GPG signed file
|  JAR        | Java archive format (same as ZIP)
|  Docker     | Docker tarball image

The following formats, which were in Binwalk Enterprise, are **not** currently supported. We will be adding support for some of them going forward.

| File Format   | Description
| ------------- | -----------
|  LZO          |  LZO compression
|  7z           |  7zip archive format
|  EXT          |  EXT file system
|  ISO          |  ISO9660 file system
|  UEFI         |  UEFI firmare
|  RomFS        |  RomFS file system
|  CAB          |  Microsoft cabinet archive format
|  Android      |  Android sparse image format
|  QNX          |  QNX file system
|  QNX6         |  QNX6 file system
|  STAR         |  STAR archive format
|  DPKG         |  Debian package archive format
|  Linux Kernel |  Linux kernel version ID
|  SquashFSv3   |  SquashFS version 3 file system
