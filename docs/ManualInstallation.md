---
permalink: /ManualInstallation.html
title: Manual Installation
description: the flat-pack Kiea instructions, written in Kerbalese, unusally present
# layout: bare
tags: installation,directions,page,kerbal,ksp,zer0Kerbal,zedK
---

<!-- ManualInstallation.md v1.1.7.0
Taerobee (TBEE)
created: 01 Oct 2019
updated: 18 Apr 2022 -->

<!-- based upon work by Lisias -->

# Taerobee (TBEE)

[Home](./index.md)

Taerobee (TBEE) adds some early rocket engines, such as Aerobee and X-4 (V-2 sounding rocket)

## Installation Instructions

### Using CurseForge/OverWolf app or CKAN

You should be all good! (check for latest version on CurseForge)

### If Downloaded from CurseForge/OverWolf manual download

To install, place the `Taerobee` folder inside your Kerbal Space Program folder:

* **REMOVE ANY OLD VERSIONS OF THE PRODUCT BEFORE INSTALLING**, including any other fork:
  * Delete `<KSP_ROOT>/GameData/Taerobee`
* Extract the package's `Taerobee/` folder into your KSP's as follows:
  * `<PACKAGE>/Taerobee` --> `<KSP_ROOT>/GameData`
    * Overwrite any preexisting file(s).
  * you should end up with `<KSP_ROOT>/GameData/Taerobee`

### If Downloaded from SpaceDock / GitHub / other

To install, place the `GameData` folder inside your Kerbal Space Program folder:

* **REMOVE ANY OLD VERSIONS OF THE PRODUCT BEFORE INSTALLING**, including any other fork:
  * Delete `<KSP_ROOT>/GameData/Taerobee`
* Extract the package's `GameData/` folder into your KSP's as follows:
  * `<PACKAGE>/GameData` --> `<KSP_ROOT>`
    * Overwrite any preexisting file(s).
  * you should end up with `<KSP_ROOT>/GameData/Taerobee`

## The following file layout must be present after installation

```markdown
<KSP_ROOT>
  + [GameData]
    + [Taerobee]
      + [Compatibility]
        ...
      + [Localization]
        ...
      + [Parts]
        ...
      * #.#.#.#.htm
      * changelog.md
      * CC-BY-ND-3.0.txt
      * readme.htm
      * Taerobee.version
    ...
  * KSP.log
  * PartDatabase.cfg
  ...
```

### Dependencies

* none
