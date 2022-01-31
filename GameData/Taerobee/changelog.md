| modName | Taerobee (TBEE)                                                |
| ------- | -------------------------------------------------------------- |
| license | CC-BY-ND-3.0                                                   |
| website | (https://forum.kerbalspaceprogram.com/index.php?/topic/205846) |
| author  | Tantares (Beale) and zer0Kerbal                                |

# Version 1.4.0.0 - Mexican Waterfalls Adapted - 2022-01-31 [KSP 1.12.2]

* 28 Jan 2022
* Release for Kerbal Space Program [KSP 1.12.x] 

## DO A CLEAN INSTALL: DELETE EXISTING THEN RE-INSTALL

---

## Waterfall Effects

* Create <EnginesPlumeSWE.cfg>
* Add stock waterfall effects
* Thank you! 🚀 - @JamesErvin-5
* Work-In-Progress
* Requires to use:
  * Waterfall
  * Stock Waterfall Effects
* Closes #52 - Stock Waterfall Effects

## Localization

* Create <es-mx.cfg>
* Adds Mexican translation - thank you - @JamesErvin-5 ⚽
* closes #50
* updates #6

## Lint Compatibility Patches

* closes #65 - Lint Compatibility Patches
* [Little-Leo.cfg] v1.0.1.0
  * make footer one line
  * closes #66 - [Little-Leo.cfg] v1.0.1.0
* [Aerobee-jr.cfg] v1.0.1.0
  * make footer one line
  * closes #67 - [Aerobee-jr.cfg] v1.0.1.0
* Update [EnginesPlumeSWE.cfg] v1.0.1.0
  * Add header/footer
  * Add license (for now it is CC BY-SA 3.0 Unported)
  * Add `,StockWaterfallEffects` to the :NEEDS
  * Thank you to @JamesErvin-5 for submitting these patches
  * closes #68 - Update [EnginesPlumeSWE.cfg] v1.0.1.0

## Update X1

| ***X1***  |          | ***diameter (m)*** | ***height (m)*** | ***math*** | ***radius (m)*** | ***m²*** | ***Liters*** |
| --------- | -------- | ------------------ | ---------------- | ---------- | ---------------- | -------- | ------------ |
| X1-body   | cylinder | 1.77               | 2.39             | πr²h       | 0.885            | 5.88077  | 5880.78      |
| X1-crew   | cylinder | 1.25               | 2.64             | πr²h       | 0.625            | 3.23977  | 3239.77      |
| X1-engine | cylinder | 0.625              | 0.74             | πr²h       | 0.3125           | 0.22703  | 227.03       |
| X1-tail   | cone     | 1.25               | 3.28             | (πr²h)/3   | 0.625            | 1.34172  | 1341.73      |

* closes #69 - Update X1

* [tbee-x1-body]
  * Add
    * DRAG_CUBE
    * [ModuleCargoPart]
      * type = cylinder
      * radius = 0.885m
      * height = 2.39m
      * volume = 5.880772 m³  // 2.932971
      * m³ x 1000L = m³
      * packedVolume = 6000
  * closes #70 - [tbee-x1-body]
* [tbee-x1-tail]
  * Add
    * DRAG_CUBE
    * [ModuleCargoPart]
      * type = cone
      * radius = 0.625m
      * height = 3.28m
      * volume = 1.341722 m³
      * m³ x 1000L = m³
      * packedVolume = 1350
  * closes #71 - [tbee-x1-tail]
* [tbee-x1-crew]
  * Add
    * DRAG_CUBE
    * [ModuleCargoPart]
      * type = cylinder
      * radius = 0.625 m
      * height = 2.64 m
      * volume = 0.876033 m³
      * m³ x 1000L = m³
      * packedVolume = 1000
  * closes #72 - [tbee-x1-crew]
* [tbee-x1-engine]
  * Add
    * DRAG_CUBE
    * [ModuleCargoPart]
      * type = cylinder
      * radius = 0.625 m
      * height = 0.74 m
      * volume = 0.242236 m³
      * m³ x 1000L = m³
      * packedVolume = 300
  * closes #73 - [tbee-x1-engine]

## Update Bumper

| ***file name***      |           | ***diameter (m)*** | ***height (m)*** | ***width (m)*** | ***math*** | ***radius (m)*** | ***m²*** | ***Liters*** |
| :------------------- | :-------: | -----------------: | ---------------: | :-------------: | ---------: | ---------------: | -------: | -----------: |
| bumper-body          | cylinder  |              0.625 |             1.09 |                 |       πr²h |           0.3125 |  0.33441 |       334.41 |
| bumper-control       | cylinder  |              0.625 |             0.09 |                 |       πr²h |           0.3125 |  0.02761 |        27.62 |
| bumper-engine        | cylinder  |              0.625 |             1.34 |                 |       πr²h |           0.3125 |  0.41111 |       411.11 |
| bumper-engine-unclad | cylinder  |              0.625 |             1.33 |                 |       πr²h |           0.3125 |  0.40804 |       408.04 |
| bumper-fin           | rectangle |               0.46 |             1.42 |      0.02       |      L*H*W |             0.23 |  0.01306 |        13.07 |
| bumper-nose          |   cone    |              0.625 |             2.36 |                 |   (πr²h)/3 |           0.3125 |  0.24135 |       241.35 |

* closes #77 - Update Bumper

* [bumper-body.cfg]
  * rename part cfg to use hyphen
  * Add
    * DRAG_CUBE
    * [ModuleCargoPart]
      * type = cylinder
      * radius = 0.3125m
      * height = 1.09m
      * volume = 0.33441 m³
      * m³ x 1000L = m³
      * packedVolume = 350
      * stackableQuantity = 2
  * closes #79 - [bumper-body.cfg]
* [bumper-control.cfg]
  * rename part cfg to use hyphen
  * uncomment [ModuleReactionWheel]
    * Pitch/Yaw/Roll Torque = 0.1
    * consumes [ElectricChange] at a rate of 0.1
  * Add
    * DRAG_CUBE
    * [ModuleCargoPart]
      * type = cylinder
      * radius = 0.3125m
      * height = 0.09m
      * volume = 0.02761 m³
      * m³ x 1000L = 27.62 m³
      * packedVolume = 30
      * stackableQuantity = 10
  * closes #80 - [bumper-control.cfg.cfg]
* [bumper-engine.cfg]
  * rename part cfg to use hyphen
  * Add
    * DRAG_CUBE
    * [ModuleCargoPart]
      * type = cylinder
      * radius = 0.3125m
      * height = 1.34m
      * volume = 0.41111 m³
      * m³ x 1000L = 411.11 m³
      * packedVolume = 425
      * stackableQuantity = 2
  * closes #81 - [bumper-engine.cfg]
* [bumper-engine-unclad.cfg]
  * rename part cfg to use hyphen
  * Add
    * DRAG_CUBE
    * [ModuleCargoPart]
      * type = cylinder
      * radius = 0.3125m
      * height = 1.33m
      * volume = 0.40804 m³
      * m³ x 1000L = 408.04 m³
      * packedVolume = 415
      * stackableQuantity = 2
  * closes #82 - [bumper-engine-unclad.cfg]
* [bumper-fin.cfg]
  * rename part cfg to use hyphen
  * Add
    * DRAG_CUBE
    * [ModuleCargoPart]
      * type = rectangle
      * x = 0.46m
      * y = 1.42m
      * z = 0.02m
      * volume = 0.01306 m³
      * m³ x 1000L = 13.07 m³
      * packedVolume = 14
      * stackableQuantity = 12
  * closes #83 - [bumper-fin.cfg]
* [bumper-nose.cfg]
  * rename part cfg to use hyphen
  * Add
    * DRAG_CUBE]
    * [ModuleCargoPart]
      * type = cone
      * radius = 0.3125m
      * height = 2.36m
      * volume = 0.24135 m³
      * m³ x 1000L = 241.35 m³
      * packedVolume = 250
      * stackableQuantity = 4
  * closes #84 - [bumper-nose.cfg]

## Update Taerobee

| ***Taerobee***           |            | ***diameter (m)*** | ***height (m)*** | ***width (m)*** |     ***math***     | ***radius (m)*** | ***m²*** | ***Liters*** |
| :----------------------- | :--------: | -----------------: | ---------------: | --------------: | :----------------: | ---------------: | -------: | -----------: |
| taerobee-adapter-short   | trunc.cone |              0.625 |              0.1 |         0.15625 | (1/3)πh (r²+rR+R²) |           0.3125 |  0.01790 |         17.9 |
| taerobee-adapter-tall    | trunc.cone |              0.625 |              0.3 |         0.15625 | (1/3)πh (r²+rR+R²) |           0.3125 |  0.05369 |        53.69 |
| taerobee-aerobee         |  cylinder  |              0.625 |             0.43 |                 |        πr²h        |           0.3125 |  0.13192 |       131.93 |
| taerobee-control         |  cylinder  |              0.625 |              0.1 |                 |        πr²h        |           0.3125 |  0.03068 |        30.68 |
| taerobee-decoupler       |  cylinder  |              0.625 |             0.19 |                 |        πr²h        |           0.3125 |  0.05829 |         58.3 |
| taerobee-despin          |  cylinder  |              0.625 |              0.1 |                 |        πr²h        |           0.3125 |  0.03068 |        30.68 |
| taerobee-fin-large       | rectangle  |               0.36 |             0.72 |            0.02 |       L*H*W        |           0.1800 |  0.00518 |         5.19 |
| taerobee-fin-small       | rectangle  |               0.37 |             0.16 |            0.04 |       L*H*W        |           0.1850 |  0.00237 |         2.37 |
| taerobee-nosecone        |    cone    |              0.625 |             0.98 |                 |      (πr²h)/3      |           0.3125 |  0.10022 |       100.23 |
| taerobee-parachute       |    cone    |              0.625 |              0.3 |                 |      (πr²h)/3      |           0.3125 |  0.03068 |        30.68 |
| taerobee-science         |  cylinder  |              0.625 |              0.3 |                 |        πr²h        |           0.3125 |  0.09204 |        92.04 |
| taerobee-sustainertank-3 |  cylinder  |              0.625 |             2.88 |                 |        πr²h        |           0.3125 |  0.88357 |       883.58 |
| taerobee-tinytim         |  cylinder  |              0.625 |             1.14 |                 |        πr²h        |           0.3125 |  0.34975 |       349.75 |

* closes #78 - Update Taerobee

* [taerobee-adapter-short.cfg]
  * Create part based on Squad's adapterSmallMiniShort
    * [rescaleFactor] = 0.5
    * [bulkheadProfiles] = size00,size0
    * keep variants
  * add @Thumb
  * Update Localization - <en-us.cfg>
  * Add
    * DRAG_CUBE]
    * [ModuleCargoPart]
      * type = trunc.cone
      * radius = 0.3125 m
      * Radius = 0.15625 m
      * height = 0.1 m
      * volume = 0.0179 m³
      * m³ x 1000L = 17.9 m³
      * packedVolume = 18
      * stackableQuantity = 20
  * closes #87 - [taerobee-adapter-short.cfg]
* [taerobee-adapter-tall.cfg]
  * Create part based on Squad's adapterSmallMiniTall
    * [rescaleFactor] = 0.5
    * [bulkheadProfiles] = size00,size0
    * keep variants
  * add @Thumb
  * Update Localization - <en-us.cfg>
  * Add
    * DRAG_CUBE]
    * [ModuleCargoPart]
      * type = trunc.cone
      * radius = 0.3125 m
      * Radius = 0.15625 m
      * height = 0.3 m
      * volume = 0.05369 m³
      * m³ x 1000L = 53.69 m³
      * packedVolume = 55
      * stackableQuantity = 8
  * closes #88 - [taerobee-adapter-tall.cfg]
* [taerobee-aerobee.cfg]
  * rename part cfg to use hyphen
  * change [bulkheadProfiles] from size0 to size00
  * FX randsomed until [ModuleEnginesFX] changed back to [ModuleEngines]; FX returned unharmed
  * Added [EngineType] = LiquidFuel to [ModuleEngines]]
  * Add
    * DRAG_CUBE]
    * [ModuleCargoPart]
      * type = cylinder
      * radius = 0.3125 m
      * height = 0.43 m
      * volume = 0.13192 m³
      * m³ x 1000L = 131.93 m³
      * packedVolume = 150
      * stackableQuantity = 5
  * closes #89 - [taerobee-aerobee.cfg]
* [taerobee-control.cfg]
  * Rename part cfg to use hyphen
  * Change [bulkheadProfiles] from size0 to size00
  * Change [ModuleCommand] EC consumption from 0.001 to 0.006 re: early tech worse than 0.005 (21.5/h)
  * Add [ModuleSAS] - no level
  * Add [ModuleReactionWheel]
    * PitchTorque = 0.5
    * YawTorque = 0.5
    * RollTorque = 0.5
    * torqueResponseSpeed = 11
    * consumes [ElectricCharge] at a rate of 0.01 re: early tech - worse than 0.0003
  * Updates[ModuleDataTransmitter]
    * [packetInterval] set to 1.0, was 0.6
    * [packetSize] set to 2, was 1
    * [antennaPower] set to 5000, was 50000
  * Resource [ElectricCharge] upped to 75, was 5 re: same size as Z-100 but earlier tech and other things in part
  * Add
    * DRAG_CUBE]
    * [ModuleCargoPart]
      * type = cylinder
      * radius = 0.3125 m
      * height = 0.1 m
      * volume = 0.03068 m³
      * m³ x 1000L = 30.68 m³
      * packedVolume = 32
      * stackableQuantity = 12
  * closes #90 - [taerobee-control.cfg]
* [taerobee-decoupler.cfg]
  * rename part cfg to use hyphen
  * Change [bulkheadProfiles] from size0,srf to size00,srf
  * Add
    * DRAG_CUBE]
    * [ModuleCargoPart]
      * type = cylinder
      * radius = 0.3125 m
      * height = 0.19 m
      * volume = 0.05829 m³
      * m³ x 1000L = 58.3 m³
      * packedVolume = 60
      * stackableQuantity = 8
  * closes #91 - [taerobee-decoupler.cfg]
* [taerobee-despin.cfg]
  * rename part cfg to use hyphen
  * change [bulkheadProfiles] from size0 to size00
  * Resource [MonoPropellant] amount changed to 3.0 from 1.5
  * [ModuleSAS] consumption rate updated from 0.05 to 0.25
  * Add
    * DRAG_CUBE]
    * [ModuleCargoPart]
      * type = cylinder
      * radius = 0.3125 m
      * height = 0.1 m
      * volume = 0.03068 m³
      * m³ x 1000L = 30.68 m³
      * packedVolume = 35
      * stackableQuantity = 10
  * closes #92 - [taerobee-despin.cfg]
* [taerobee-fin-large.cfg]
  * rename part cfg to use hyphen
  * Add
    * DRAG_CUBE]
    * [ModuleCargoPart]
      * type = rectangle
      * x = 0.36m
      * y = 0.72m
      * z = 0.02m
      * volume = 0.00518 m³
      * m³ x 1000L = 5.19 m³
      * packedVolume = 6
      * stackableQuantity = 12
  * closes #93 - [taerobee-fin-large.cfg]
* [taerobee-fin-small.cfg]
  * rename part cfg to use hyphen
  * Add
    * DRAG_CUBE]
    * [ModuleCargoPart]
      * type = rectangle
      * x = 0.37m
      * y = 0.72m
      * z = 0.04m
      * volume = 0.00237 m³
      * m³ x 1000L = 2.37 m³
      * packedVolume = 3
      * stackableQuantity = 20
  * closes #94 - [taerobee-fin-small.cfg]
* [taerobee-nosecone.cfg]
  * rename part cfg to use hyphen
  * change [bulkheadProfiles] from size0 to size00
  * Add
    * DRAG_CUBE]
    * [ModuleCargoPart]
      * type = cone
      * radius = 0.3125 m
      * height = 0.98 m
      * volume = .010022 m³
      * m³ x 1000L = 100.25 m³
      * packedVolume = 125
      * stackableQuantity = 4
  * closes #95 - [taerobee-nosecone.cfg]
* [taerobee-parachute.cfg]
  * rename part cfg to use hyphen
  * change [bulkheadProfiles] from size0 to size00
  * Updated [attachRules] from 1,0,1,0,0 to 1,0,0,1,0
  * Added [buoyancyUseCubeNamed] = PACKED
  * Added FX
    * [fx_gasBurst_white] = 0.0, 0.0, 0.0, 0.0, 1.0, 0.0, decouple
    * [sound_decoupler_fire] = decouple
  * Updated [maxTemp] from 2000 to 2250 re: prototype
  * Added [emissiveConstant] = 0.7
  * Changed [crashTolerence] from 12 to 8
  * Added [preferredStage] = PARACHUTESTAGE
  * [ModuleParachute]
    * [clampMinAirPressure] = 0.04
    * [deploymentSpeed] set to 0.12 was 1
    * [semiDeploymentSpeed] set to 0.5 was 1
    * [chuteMaxTemp] = 650
  * [ModuleDragModifier]
    * [dragModifier] set to 1.25 was 1
  * [ModuleDecouple]
    * [ejectionForcePercent] = 100
    * [fxGroupName] = decouple
    * [menuName] = #TBEE-decoup-menu
    * [stagingEnableText] = #TBEE-decoup-enable
    * [stagingDisableText] = #TBEE-decoup-disable
  * Added [ModuleTestSubject], copied from MK1
  * Add
    * DRAG_CUBE]
    * [ModuleCargoPart]
      * type = cone
      * radius = 0.3125 m
      * height = 0.3 m
      * volume = 0.03068 m³
      * m³ x 1000L = 30.68 m³
      * packedVolume = 35
      * stackableQuantity = 12
  * closes #96 - [taerobee-parachute.cfg]
* [taerobee-science.cfg]
  * rename part cfg to use hyphen
  * change [bulkheadProfiles] from size0 to size00
  * Add
    * DRAG_CUBE]
    * [ModuleCargoPart]
      * type = cylinder
      * radius = 0.3125 m
      * height = 0.3 m
      * volume = 0.09204 m³
      * m³ x 1000L = 92.04 m³
      * packedVolume = 100
      * stackableQuantity = 4
  * closes #97 - [taerobee-science.cfg]
* [taerobee-sustainertank-3.cfg]
  * rename part cfg to use hyphen
  * change [bulkheadProfiles] from size0 to size00
  * Add
    * DRAG_CUBE]
    * [ModuleCargoPart]
      * type = cylinder
      * radius = 0.3125 m
      * height = 2.88 m
      * volume = 0.88357 m³
      * m³ x 1000L = 883.58 m³
      * packedVolume = 900
      * stackableQuantity = 1
  * closes #98 - [taerobee-sustainertank-3.cfg]
* [taerobee-tinytim.cfg]
  * rename part cfg to use hyphen
  * change [bulkheadProfiles] from size0 to size00
  * FX randsomed until [ModuleEnginesFX] changed back to [ModuleEngines]; FX returned unharmed
  * Added [EngineType] = SolidBooster to [ModuleEngines]
  * ADD FX
    * [fx_exhaustSparks_yellow] = 0.0, -0.17, 0.0, 0.0, 1.0, 0.0, running
    * [fx_smokeTrail_medium] = 0.0, -0.17, 0.0, 0.0, 1.0, 0.0, running
    * [sound_explosion_low] = flameout
  * Adjust [entryCost] = 50 from 0
  * Change [category] = Engine from Propulsion
  * Add [heatConductivity] = 0.06 note: 1/2 default
  * [skinInternalConductionMult] = 4.0
  * [emissiveConstant] = 0.5 note: yes, it's white. But let's claim it's an emissive white...
  * Change
    * [maximum_drag] from 0.3 to 0.2
    * [crashTolerance] from 8 to 7
    * [maxTemp] from 3400 to 2000
  * Add [ModuleJettison]
  * Adjust [SolidFuel] resource
    * [amount] to 35 initially 10
    * [maAmount] to 35 initially 10
    * math:
      * volume of Part in L = 349.75
      * divide by 50 for units (ratio taken from stock solidBooster RT-10)
      * multiple by 5 units per unit for SolidFuel
      * = 34.95 units of [SolidFuel]
  * Add
    * DRAG_CUBE]
    * [ModuleCargoPart]
      * type = cylinder
      * radius = 0.3125 m
      * height = 1.14 m
      * volume = 0.34975 m³
      * m³ x 1000L = 349.78L
      * packedVolume = 400
      * stackableQuantity = 1
  * closes #99 - [taerobee-tinytim.cfg]

## Status

* #25 - 7ranceaddic7 adoption- contributed by zer0Kerbal
* #26 - merge in tythos adoption- contributed by zer0Kerbal
* #27 - Peter-JY-a adoption- contributed by zer0Kerbal
* #28 - Peter-JY-100 adoption- contributed by zer0Kerbal
* #29 - tk-313 adoption- contributed by zer0Kerbal
* #30 - 1.3.0.0 archive adoption- contributed by zer0Kerbal
* #32 - 1.3.9.9 adoption adoption- contributed by zer0Kerbal
* #49 - Create es-mx.cfg- contributed by JamesErvin-5
* #51 - Create EnginesPlumeSWE.cfg issue: compatibility/patch, issue: config, type: feature, type: request, state: approved- contributed by JamesErvin-5
* #53 - upstream changes type: upstream- contributed by zer0Kerbal
* #74 - X1 updates issue: config, type: fix- contributed by zer0Kerbal
* #85 - Revert &quot;Update Bumper&quot;- contributed by zer0Kerbal
* #86 - Update Bumper issue: config- contributed by zer0Kerbal
* #101 - Update taerobee 1.4.0.0 issue: config- contributed by zer0Kerbal
* #1 - Adoption Legal MumboJumbo adoption
* #2 - Adoption Documentation adoption
* #3 - Release 1.3.9.9-adoption adoption
* #4 - Adoption - GitHub adoption
* #5 - Adoption - social media adoption
* #7 - Localization - English (United States) &lt;en-us.cfg&gt; 
* #8 - Localization - Russian (&#1056;&#1091;&#1089;&#1089;&#1082;&#1080;&#1081;) &lt;ru.cfg&gt; 
* #23 - Merge in other forks
* #33 - Thumbnails adoption
* #34 - add antenna to both control parts
* #35 - move art assets to Assets adoption
* #36 - Update decoupler adoption
* #37 - update English Localization &lt;en-us.cfg&gt; adoption
* #39 - Update sustainer tank adoption
* #40 - Update Bumper body adoption
* #41 - Update Bumper engine adoption
* #42 - Update Bumper engine unclad adoption
* #43 - Update Bumper Nose adoption
* #44 - Update X1 Body adoption
* #45 - Update X1 Tail adoption

# 1.3.9.9-adoption - Return to flight line [KSP 1.12.2] [ 03-12-2021]

## Update Compatibility Patches

* [Little-Leo.cfg] v1.0.1.0
  - header/footer
  - :FOR[Taerobee]
  - name

* [Aerobee-jr.cfg] v1.0.1.0
  - header/footer
  - :FOR[Taerobee]
  - name
  
## Update Localization

* English <en-us.cfg>
* Russian <ru.cfg>
* [taerobee.science.cfg]
  - localize experiments

## Update
* file names
  - underscore to dash '_' --> '-'
  - change to all lowercase
  - add 'tbee-' prefix
* part names
  - underscore to dash '_' --> '-'
* ModuleEngines --> ModuleEnginesFX
* add key = 7 0.001 to atmosphereCurve
* ModuleCommand

## Art Assets
* moved into GameData/Taerobee/Assets
* .mbm --> .dds in model files
* convert to .png and archive .mbm files

## Update INSTALL.md

## Update decoupler

* add explosionPotential = 0.1
* update FX from 'activate' to 'decouple'
* adjust angular drag from 1.0 to 0.25
* add
  - stagingIcon = DECOUPLER_HOR
  - ejectionForcePercent = 100
  - fxGroupName = decouple
  - menuName = Decouple Top Node
  - stagingEnableText = #TBEE-decoup-enable
  - stagingDisableText = #TBEE-decoup-disable
  - menuName = #TBEE-decoup-menu
* update #36

## update English Localization <en-us.cfg>

* add
  - #TBEE-taerobee-aerobee-tags
  - #TBEE-taerobee-control-tags
  - #TBEE-taerobee-decoupler-tags
  - #TBEE-taerobee-despin-tags
  - #TBEE-taerobee-fin-large-tags
  - #TBEE-taerobee-nosecone-tags
  - #TBEE-taerobee-parachute-tags
  - #TBEE-taerobee-science-tags
  - #TBEE-taerobee-fin-small-tags
  - #TBEE-taerobee-Tank-Sustainer-3
  - #TBEE-taerobee-TinyTim-tags [incomplete]
  - #TBEE-decoup-enable = Decoupler: Enabled
  - #TBEE-decoup-disable = Decoupler: Disabled
  - #TBEE-decoup-menu = Decoupler: All Nodes
  - #TBEE-Thermometer-open = Thermometer: Open Doors
  - #TBEE-Thermometer-clos = Thermometer: Close Doors
  - #TBEE-Thermometer-togl = Thermometer: Toggle Doors
  - #TBEE-Barometer-open = Barometer: Open Doors
  - #TBEE-Barometer-clos = Barometer: Close Doors
  - #TBEE-Barometer-togl = Barometer: Toggle Doors
* updates #31 
* closes #37

## Update Russian Localization <ru.cfg>

* add [incomplete - needs translation]
  - #TBEE-taerobee-TinyTim-tags
  - #TBEE-decoup-enable = Decoupler: Enabled
  - #TBEE-decoup-disable = Decoupler: Disabled
  - #TBEE-decoup-menu = Decoupler: All Nodes
  - #TBEE-Thermometer-open = Thermometer: Open Doors
  - #TBEE-Thermometer-clos = Thermometer: Close Doors
  - #TBEE-Thermometer-togl = Thermometer: Toggle Doors
  - #TBEE-Barometer-open = Barometer: Open Doors
  - #TBEE-Barometer-clos = Barometer: Close Doors
  - #TBEE-Barometer-togl = Barometer: Toggle Doors
* updates #31 
* closes #38

## Update sustainer tank

* change
  - category = FuelTank from Propulsion
  - maximum_drag = 0.2 from 0.3
  - maxTemp = 2000 from 3400 
* add
  - breakingForce = 50
  - breakingTorque = 50
  - fuelCrossFeed = true
* closes #39

## Update Bumper body

* change
  - category = FuelTank from Propulsion
* closes #40

## Update Bumper engine

* add 
  - FXModuleAnimateThrottle
  - heatConductivity = 0.06
  - skinInternalConductionMult = 4.0
  - emissiveConstant = 0.8
  - key = 7 0.001
* update ModuleEngines to ModuleEnginesFX
* closes #41

## Update Bumper engine unclad

* add 
  - FXModuleAnimateThrottle
  - heatConductivity = 0.06
  - skinInternalConductionMult = 4.0
  - emissiveConstant = 0.8
  - key = 7 0.001
* update ModuleEngines to ModuleEnginesFX
* closes #42

## Update Bumper Nose

* change
  - category = FuelTank from Propulsion
* closes #43

## Update X1 Body

* change
  - category = FuelTank from Propulsion
* closes #44

## Update X1 Tail

* change
  - category = FuelTank from Propulsion
* closes #45

Change Log of Taerobee (Peter-JY/Taerobee)
=====================================================

1.0.0
* Reposted Taerobee a.b.c, and change the version number to 1.0.0
* Make it compatible with KSP 1.4.0~1.9.1
* Add the original license of it

*I found the original version number, but I temporarily forgot it. I will add it the next time I update the version.