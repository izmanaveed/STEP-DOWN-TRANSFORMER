# STEP-DOWN-TRANSFORMER

## Problem Statement 
To design and implement a step-down transformer (230 V to 18 V) and perform open circuit test to find out required parameters as well. 

## Working 
The two voltages, between line 1 and neutral and between neutral and line 2 can be named as VA and VB respectively. Then the mathematical relation of these two voltages shows that they are dependent upon the primary voltage as well as the turn ration of the transformer.
VA = (NA / NP) * VP
VB = (NB / NP) * VP
One thing that should be noted here is that both the outputs VA and VB respectively are equal in magnitude but opposite in direction, which means that they are 180 degrees out of phase with each other. For this purpose, we also use a full wave rectifier with a center tapped transformer, to make both the voltages in phase with each other.

## Calculations
Assuming Vp= 240V 
We have designed a step-down transformer from 240 V to 18 V so, Vs= 18V
Core Area = CA= 3.8cm x 5cm = 19 cm2
To calculate Turns/Volt:
TPV = 1 / (4.44 × 10-4 × CA × Flux Density × AC frequency)
Where, 
CA = 19 cm2
Flux density = 1Wb/sq.m
AC frequency = 50 Hz
So we get TPV = 2.37
We have taken TPV = 2.5 to compensate for any losses that may occur. 

## DESIGN SPECIFICATIONS SUMMARY
![image](https://github.com/izmanaveed/STEP-DOWN-TRANSFORMER/assets/59065717/6cf73881-7201-4c0f-8e9e-bacfc8171bae)

## Simulated Results

### a)FROM CALCULATED VALUES

V1/V2 = N1/N2
(V1/V2)2  = L1/L2 = N1/N2
L1/L2 = (600)2 / (45)2 = 360000 / 2025 
![image](https://github.com/izmanaveed/STEP-DOWN-TRANSFORMER/assets/59065717/88e7e2a5-824c-4603-913d-cb686d932d9f)
![image](https://github.com/izmanaveed/STEP-DOWN-TRANSFORMER/assets/59065717/9bcc4922-479b-4b95-866e-fad5e048c32c)

### b)FROM MEASURED VALUES

V1/V2 = N1/N2
(V1/V2)2  = L1/L2 = N1/N2
L1/L2 = (600)2 / (40)2 = 360000 / 1600 
Vp = 238.96V
Vs = 17.95V
![image](https://github.com/izmanaveed/STEP-DOWN-TRANSFORMER/assets/59065717/fd662afe-d023-454b-8391-722832a2d8a5)
![image](https://github.com/izmanaveed/STEP-DOWN-TRANSFORMER/assets/59065717/12ea15a9-a408-43f6-b82a-8f5497ec6734)
Vp = 239.63V
Vs = 15.97V

## Measured Results (Practical Implementation)

### OPEN-CIRCUIT TEST
Ioc = 0.1 A
Voc = 240 V
Poc = 20 W
S= VI = 24 VA
pf= cosӨ = Poc/VocIoc = 0.833
Ө = 33.55o
sinӨ = 0.55
Rc = V/IcosӨ = 2881.15 Ω
Xm = V/IsinӨ = 4363.63 H

## Problems Faced
1. A major problem faced while making this project was that length of wire for secondary windings was insufficient which resulted in less number of turns on secondary as compared to the required value i.e. instead of 45 turns, only 40 turns 1.were possible. The effect of this was that the step-down output voltage was at 15.2 V instead of 18 V. 
2. There was lots of vibration being produced and the transformer heated up. This was due to less insulations between the primary and secondary windings. This issue was resolved by adding another layer of insulating material between the windings.

## Final Result 
We have designed a center – tapped step-down transformer that steps down voltage from 240 V to 18 V.
![image](https://github.com/izmanaveed/STEP-DOWN-TRANSFORMER/assets/59065717/5b659923-54b6-49ca-accf-c2f8201b24c6)



