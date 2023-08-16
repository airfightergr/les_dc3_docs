# Liveries Concept

We are introducing a new concept about how liveries are handled in our aircraft. The rationale is to honour the aircraft, as the first airliner, which also fought in WWII, but the iconic users, via the liveries.
To do that, we handle as every livery as a unique airframe. 

## Liveries as Airframes

You must think that by selecting a livery to fly, you are also selecting a different airframe. For example, switching from **Buffalo Airways** to **Duggy**, is like climbing on a different aircraft, and not just changing the paint!
From now on, in this page the word **Airframe** will be used instead of livery. 

!!! note "NOTE"
    Currently, changing livery, does not reset the flight, as it should do, since you switch airframes, due to not be able to achieve stable transition without crashes. But we are looking to implement it in a future update. 

!!! danger "CAUTION"
    Switching liveries while flying, might have disastrous consequences! The new airframe options might command to load the aircraft cold and dark, which won't be nice while you are flying!<br>
    **Always switch liveries on the ground!**

Here are the properties:

1. We have implemented a maintenance system that is tracked, per aircraft, per airframe. Each time you fly, the hours are logged to the specific airframe. So the airframe hours and maintenance intervals, are counted per airframe.
For example, if you fly frequently with one airframe, and then select another one, that you have months to fly with, you'll find the batteries discharged.
2. The options, you choose for specific airframe, are stored only for this airframe.
3. Persistence (if you select the aircraft to load as was after the last flight), is tracked per airframe.


## Instructions for Painters

Those who want to create liveries for DC3, should have a few things in mind. 

- We will provide you a paintkit, for both Photoshop and Substance Painter.
- Each livery requires a ***.ini*** file for data and information to be stored. We will provide you with a file that you can edit it.
- The liveries' ***.ini*** files are located in the ***X-Plane 12/Output/DC3*** folder.
- The file for your livery should be named exactly as the livery folder. For example is the livery folder is named **United Airlines**, the file should have the name **United Airlines.ini**.
- You should ship your livery with the ini file. We suggest to create a zip with the structure below:

```
zip file
    |
     - Aircraft/X-Aviation/DC3/liveries/ your livery folder here
    |
     - Output/DC3/ your ini file here  

```


!!! hint "INFO"
    If you load DC-3 in X-Plane, with your livery folder in place, and without creating or adding the required ***.ini*** file, will create one for you, replicated the default's livery one. Then you can edit this file.


## INI File configuration

The ***.ini*** file has 4 sections

### Data

You **must** edit those 3 fields, to make your livery unique! 

```
[DATA]
TAIL_NUMBER=VH-LES
DESCRIPTION=Released on April 1, 2012
OPERATOR=Leading Edge Simulations Modern
```
  - TAIL_NUMBER: The tail number of your livery. We are using it to set the respective X-Plane dataref. 
  - DESCRIPTION: Add a very short description for your livery. *Note:* Use only 1 line of text.
  - OPERATOR: Aircraft's operator name.


### Initialization

Here, are stored various values (options, fuel quantities, etc.), used when the aircraft loads. You **do not need** to edit those values. 

```
[INIT]
OPT_autopilotMode=0
OPT_diff_throttles=0
OPT_diff_throttles_sens=1
OPT_diff_brakes=1
OPT_diff_brakes_sens=2
OPT_loadingStates=3
OPT_tabletShow=1
OPT_GPS=0
TANK_L_AUX_USGAL=147.99012756348
TANK_R_AUX_USGAL=147.9958190918
TANK_L_MAIN_USGAL=184.40916442871
TANK_R_MAIN_USGAL=184.40916442871
BARO_copilot=28.020011901855
BARO_pilot=27.980010986328
ALT_copilot=99.50862121582
ALT_pilot=790.52117919922
OBS_hsi=155
OBS_pilot=215
OBS_copilot=65
```

### Maintenance

Here, are stored values regarding aircraft's maintenance status. You might want to edit the *AIRFRAME_HOURS* value, if you have information about how many hours the aircraft has flown.

If you don't have any info, a good guesstimation is: An aircraft flown for many years, should have more than 30,000 hours, and, if, have flown only for a few year, around 10,000 to 15,000 hours.

```
[MAINTENANCE]
AIRFRAME_HOURS=22403.654704473
BAT_CHARGE=716.86096191406
CHECK_1_HRS=24.661567467262
LAST_FLY_MONTH=06
ENG1_OIL_DATE=19519
CHECK_4_DATE=19519
ENG1_OVERHAUL_HRS=24.464319186153
CHECK_1_DATE=19519
ENG2_OIL_DATE=19519
ENG2_OIL_QLT=0.88
ENG1_OIL_QTY=0.75
CHECK_2_DATE=19519
HYD_FLUID_QTY=0.8
CHECK_3_DATE=19519
ENG2_SPARK_PLUG_HOURS=23.447136929509
CHECK_2_HRS=24.655210732032
ENG1_SPARK_PLUG_HOURS=24.464805187063
ENG1_OIL_HOURS=24.465238964766
ENG2_OVERHAUL_HRS=23.446452797463
LAST_FLY_YEAR=2023
ENG2_OIL_QTY=0.73
HYD_FLUID_QLY=0.87
ENG1_OIL_QLT=0.85
ENG2_OIL_HOURS=23.447537900815
LAST_FLY_DAY=22
```

### Persistent

Stores various values to used if you load the aircraft in **PERSISTENT** state. **Do not edit** those values!

```
[PERSISTENT]
R_magneto=3
navLights_sw=0
ldgLitSwRight=1
doorOpenRheo=0.8
DomeLIT_sw=0
LThrottle=0.1
lFuelBoostRheo=0.8
rFuelPressRheo=0.8
rStart_sw=0
RMixPad=0
lgRedRheo=0.8
cabinLights_sw=0
lOilPressRheo=0.8
antiColl_sw=1
LMixture=0.8
RThrottle=0.1
wingLight_sw=0
lFuelPressRheo=0.8
gpuConnRheo=0.8
rFuelSelector=4
LCarbHeat=0
XpndrMode=1
inverterSw=1
LMixPad=0
outMarkRheo=0.8
DomeLITKnob=0
RCarbHeat=0
Master_Start=0
L_magneto=3
master_magn_sw=1
inMarkRheo=0.8
noSmoking_sw=1
FltInstrLIT=0
CompassLITKnob=0
pitotPLTHeatSw=0
RMixture=0.8
rFuelBoostRheo=0.8
lGenSw=1
rVaccumRheo=0.8
pitotFOHeatSw=0
lfuelBoost_sw=1
gpuOnSw=0
LFirewallValve=1
lStart_sw=0
ldgLitSwLeft=1
lFuelSelector=2
seatBelts_sw=1
batterySw=2
RFirewallValve=1
lVaccumRheo=0.8
midMarkRheo=0.8
lEngFireRheo=0.8
masterRadio=1
rOilPressRheo=0.8
lgGreenRheo=0.8
rGenSw=1
rfuelBoost_sw=1
rEngFireRheo=0.8
```