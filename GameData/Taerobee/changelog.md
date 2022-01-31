# 1.3.9.9-adoption - Return to flight line [KSP 1.12.2] [ 03-12-2021]

## Update Compatibility Patches

- [Little-Leo.cfg] v1.0.1.0
  - header/footer
  - :FOR[Taerobee]
  - name

- [Aerobee-jr.cfg] v1.0.1.0
  - header/footer
  - :FOR[Taerobee]
  - name
  
## Update Localization

- English <en-us.cfg>
- Russian <ru.cfg>
- [taerobee.science.cfg]
  - localize experiments

## Update
- file names
  - underscore to dash '_' --> '-'
  - change to all lowercase
  - add 'tbee-' prefix
- part names
  - underscore to dash '_' --> '-'
- ModuleEngines --> ModuleEnginesFX
- add key = 7 0.001 to atmosphereCurve
- ModuleCommand

## Art Assets
- moved into GameData/Taerobee/Assets
- .mbm --> .dds in model files
- convert to .png and archive .mbm files

## Update INSTALL.md

## Update decoupler

- add explosionPotential = 0.1
- update FX from 'activate' to 'decouple'
- adjust angular drag from 1.0 to 0.25
- add
  - stagingIcon = DECOUPLER_HOR
  - ejectionForcePercent = 100
  - fxGroupName = decouple
  - menuName = Decouple Top Node
  - stagingEnableText = #TBEE-decoup-enable
  - stagingDisableText = #TBEE-decoup-disable
  - menuName = #TBEE-decoup-menu
- update #36

## update English Localization <en-us.cfg>

- add
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
- updates #31 
- closes #37

## Update Russian Localization <ru.cfg>

- add [incomplete - needs translation]
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
- updates #31 
- closes #38

## Update sustainer tank

- change
  - category = FuelTank from Propulsion
  - maximum_drag = 0.2 from 0.3
  - maxTemp = 2000 from 3400 
- add
  - breakingForce = 50
  - breakingTorque = 50
  - fuelCrossFeed = true
- closes #39

## Update Bumper body

- change
  - category = FuelTank from Propulsion
- closes #40

## Update Bumper engine

- add 
  - FXModuleAnimateThrottle
  - heatConductivity = 0.06
  - skinInternalConductionMult = 4.0
  - emissiveConstant = 0.8
  - key = 7 0.001
- update ModuleEngines to ModuleEnginesFX
- closes #41

## Update Bumper engine unclad

- add 
  - FXModuleAnimateThrottle
  - heatConductivity = 0.06
  - skinInternalConductionMult = 4.0
  - emissiveConstant = 0.8
  - key = 7 0.001
- update ModuleEngines to ModuleEnginesFX
- closes #42

## Update Bumper Nose

- change
  - category = FuelTank from Propulsion
- closes #43

## Update X1 Body

- change
  - category = FuelTank from Propulsion
- closes #44

## Update X1 Tail

- change
  - category = FuelTank from Propulsion
- closes #45

Change Log of Taerobee (Peter-JY/Taerobee)
=====================================================

1.0.0
- Reposted Taerobee a.b.c, and change the version number to 1.0.0
- Make it compatible with KSP 1.4.0~1.9.1
- Add the original license of it

*I found the original version number, but I temporarily forgot it. I will add it the next time I update the version.