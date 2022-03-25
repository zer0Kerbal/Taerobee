---
permalink: /ManualInstallation.html
title: ManualInstallation
---

<!-- ManualInstallation.md v1.1.0.0
Notes (NOTE)
created: 01 Oct 2019
updated: 02 Mar 2022 -->

<!-- based upon work by Lisias -->

# Taerobee

Taerobee (TBEE) adds some early rocket engines, such as Aerobee and X-4 (V-2 sounding rocket)

## Installation Instructions

### Using CurseForge/OverWolf app or CKAN

You should be all good! (check for latest version on CurseForge)

### If Downloaded from CurseForge/OverWolf manual download

To install, place the GameData folder inside your Kerbal Space Program folder:

* **REMOVE ANY OLD VERSIONS OF THE PRODUCT BEFORE INSTALLING**, including any other fork:
  * Delete `<KSP_ROOT>/GameData/Taerobee`
* Extract the package's `Taerobee/` folder into your KSP's as follows:
  * `<PACKAGE>/Taerobee` --> `<KSP_ROOT>/GameData/Taerobee`
    * Overwrite any preexisting file.

### If Downloaded from SpaceDock / GitHub / other

To install, place the GameData folder inside your Kerbal Space Program folder:

* **REMOVE ANY OLD VERSIONS OF THE PRODUCT BEFORE INSTALLING**, including any other fork:
  * Delete `<KSP_ROOT>/GameData/Taerobee`
* Extract the package's `GameData/` folder into your KSP's as follows:
  * `<PACKAGE>/GameData/Taerobee` --> `<KSP_ROOT>/GameData`
    * Overwrite any preexisting file.

## The following file layout must be present after installation

```markdown
<KSP_ROOT>
  [GameData]
    [Taerobee]
      [Assets]
      [Compatability]
      [Localization]
      [Parts]
      [Props]
      [Spaces]
      ...
      #.#.#.#.htm (changelog)
      Attribution.md
      Taerobee.version
      CC-BY-ND-3.0.txt
      readme.htm
    ModuleManager.dll
    ...
  KSP.log
  PastDatabase.cfg
  ...
```

### Dependencies

* none
