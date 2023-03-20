# Liveries Concept

We are introducing a new concept about how liveries are handled in our aircraft. The rationale is to honour the aircraft, as the first airliner, which also fought in WWII, but the iconic users, via the liveries.
To do that, we handle as every livery as a unique airframe. 

## Liveries as Airframes

You must think that by selecting a livery to fly, you are also selecting a different airframe. For example, switching from **Buffalo Airways** to **Duggy**, is like climbing on a different aircraft, and not just changing the paint!
From now on, in this page the word **Airframe** will be used instead of livery. Here are the properties:

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

1. **Data:**

```
[DATA]
TAIL_NUMBER=VH-LES
DESCRIPTION=Released on April 1, 2012
OPERATOR=Leading Edge Simulations Modern
```

- TAIL_NUMBER: Put the tail number of your livery. We are using it to set the respective X-Plane dataref.

