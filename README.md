# I-Class-Solid-Rocket-Motor
Design of a Sorbitol-Based I-Class Solid Rocket Motor


# Introduction

The goal is to design, manufacture and static fire a Solid Rocket Motor
with "Sugar Rocket Propellant" with a total impulse of around 450 Newton
Seconds.

# Design Process Overview

The requirement for this motor is to have a total impulse of around 450
Newton Seconds and to fit into a 38mm motor tube so through an iterative
design process a 6 grain layout was chosen along with the inner grain
diameter and the throat diameter in order to get the total impulse to
the desired target while maintaining the MEOP below 3.8 MPa and the
port-to-throat ratio higher than or equal to 2 in order to reduce the
chances of erosive burning.

## Performance

| Average Thrust:  |   430 N.   |
|:----------------:|:----------:|
|  Total Impulse:  | 486 N-sec. |
| Thrust Duration: | 1.13 sec.  |
|    Diameter:     |   38 mm    |
| Specific Impulse | 125.6 sec. |

## Physical Characteristics

|    Diameter:     | 38 mm  |
|:----------------:|:------:|
| Overall Length:  | TBD mm |
| Propellant Mass: | 395 g. |
|   Total Mass:    | TBD g. |

## Other Characteristics

|    Port-to-Throat ratio:     |  2  |
|:----------------------------:|:---:|
|    Motor length/diameter:    |  11 |
| Volumetric Loading Fraction: | 69% |

# Propellant

This motor uses Potassium Nitrate/Sorbitol (KNSB) propellant because of
its ease of casting and safety when compared to other "sugar" based
rocket propellants such as Potassium Nitrate/Sucrose (KNSU) that hardens
quickly and needs higher temperatures to fully melt.

|   Ingredients:    | Percentage |
|:-----------------:|:----------:|
| Potassium Nitrate |    65%     |
|     Sorbitol      |    35%     |

To the above, 0.2% of Sodium laureth sulfate (SLES) surfactant is added
to reduce the viscosity of the mixture to make the grain casting process
much easier.

## Preparation

The Potassium nitrate is ground to a fine powder (100 um majority
particle size) with an electric coffee grinder. Then the mixture is
weighed with a precision scale and thoroughly mixed with an electric
tumbler.

## Ignition Primer

The grains are to be coated with an ignition primer so that ignition
happens instantly throughout the motor to have a steeper pressure
increase thus having a more flat thrust curve instead of a "spike" that
can be seen in many KNSB motors.  
Ignition primer consists of:

|   Ingredients:    | Percentage |
|:-----------------:|:----------:|
| Potassium Nitrate |    80%     |
|   Carbon Powder   |    20%     |

To this mixture, isopropyl alcohol is added until the mixture gets to a
thin, paint-like consistency and then it is brushed onto all exposed
grain surfaces and is left to dry for at least 24 hours.

# Grain Design, Spacers, Inhibition & Thermal Liner

| Outer Diameter: | 32 mm |
|:---------------:|:-----:|
| Core Diameter:  | 15 mm |
|     Length:     | 60 mm |

The grain length was chosen to be 60mm to get a neutral thrust-time
curve and to follow the average grain length/diameter for 38mm solid
rocket motors (around 2).

## Casting

After the propellant has been mixed it is poured into a non-stick milk
pot with a spout that is heated to 125°C. Then it is mixed with a
silicone spatula until fully melted. When fully melted the SLES must be
added and stirred to reduce the viscosity of the mixture to facilitate
easier casting. When all of this is done, the propellant is poured into
the casting tubes that have the inhibitor and core rod already placed in
them. The coring rod must be lined with rice paper to make it easier to
demould the grain. After pouring the molten propellant, the pressure
ring must be added to cure the grain under pressure to avoid air pockets
and voids inside the grains.

## Curing

The grains are left to cure and harden for 5 days in an air-tight box
with desiccant bags. After the grains have fully cured they should be
density checked for voids and air. The target density ratio is
\><!-- -->0.95

## Grain Spacers

This design uses rubber O-Rings for spacers, specifically 28mm ID, 3mm
thickness O-Rings.

## Inhibition

The inhibitor is a two-ply poster-board glued to create a hollow
cylinder.

## Thermal Liner

The thermal liner is again a two-ply poster-board but this time a thin
layer of lacquer is applied in the inner surface to eliminate charring.

# Casing

The material for the motor casing was chosen to be 6063-T6 Aluminum
mainly because of its high tensile strength and for its relative
availability.  
The outer diameter is 38 mm to fit with readily available motor tubes
for rockets. With a thickness of 2 mm the inner diameter comes out to 34
mm.  
Using Barlow’s formula
$$P=2\cdot S\cdot \frac{t}{D}$$
where *P* is the maximum pressure that the casing can handle (MPa), *S*
is the tensile strength of the casing material (MPa), which in this case
is Aluminum-6063-T6, *t* is the wall thickness of the casing (mm) and
*D* is the outer diameter (mm).  
We can calculate that the bursting point of the casing comes to 26.3 MPa
so by knowing the MEOP of the system to be 3.67 MPa we can calculate
that the safety factor comes out to 7.2.

# Bulkhead

The bulkhead will also be machined from aluminum 6063-T6 and will be
"free floating" inside the motor held by a retaining ring.  
Sealing will be achieved with two O-Rings.

## Retaining ring - Bulkhead

The Bulkhead will be held inside the motor with an internal retaining
ring.  
A Thing to consider about retaining rings when designing cases is that
-most of the times- if you push them to their limits the groove will
fail before the retaining ring itself does.  
We can calculate the failing point of the retaining ring itself with the
formula given below:

*R**s* = *D* ⋅ *T* ⋅ *S**s* ⋅ *π*
Where *R**s* is the maximum allowable load for the retaining ring (N),
*D* is the housing diameter (mm) and *S**s* is the shear strength of the
material of the retaining ring (MPa)  
  
Using this formula we can calculate that the retaining ring will fail at
157 kN of force. If we calculate for pressure (dividing the force by the
area of the bulkhead) we can see that the motor has to reach a pressure
of 172.94 MPa for the retaining ring of the bulkhead to fail. This
result raises the problem that if the motor over-pressurizes that the
casing will fail before the bulkhead thus becoming a pipe bomb which
would be quite dangerous. But as was stated above, the groove that the
retaining ring sits into will fail with a lot less force than what is
needed to break the retaining ring itself.  
We can calculate the force needed for the groove to fail with the
formula given below:
$$G=\frac{D\cdot d\cdot Gy\cdot \pi}{q}$$
Where *G* is the maximum allowable load for the groove (N), *D* is the
housing diameter (mm), *d* is the depth of the groove (mm), *G**y* is
the yield strength of the groove material (MPa), and *q* is the
"decreasing factor", a value obtained from the value *n*/*d* using the
graph below:

<img src="q.png" style="width:40.0%" alt="image" />

Where *n* is the edge margin of the groove and *d* is the depth of the
groove as shown below:

<img src="nd.png" style="width:30.0%" alt="image" />

We can now calculate that the load needed for the bulkhead retaining
ring groove to fail is 12.11 kN, to reach that, the chamber pressure has
to be 13.3 MPa, which produces a safety factor of 3.63. This pressure is
well below the 26.31 MPa that the casing needs in order to break,
helping us ensure that in case of over-pressurization the bulkhead will
fail before the casing.

# Nozzle

The nozzle will be made from mild steel with 15 degree convergent
half-angle and 40 degree divergent half-angle and a throat diameter of
10.6 mm.  
The optimal expansion ratio for the nozzle was calculated to be 7 with
the equation below:
$$\frac{\mathrm{A}\_{ }^{\ast} }{\mathrm{A}\_{e}^{}}=\left( \frac{k+1}{2} \right)^{\frac{1}{k-1}}\left( \frac{\mathrm{P}\_{e}^{}}{\mathrm{p}\_{o}^{}} \right)^{\frac{1}{k}}\sqrt{\left( \frac{k+1}{k-1} \right)\left\[ 1-\left( \frac{\mathrm{P}\_{e}^{}}{\mathrm{P}\_{o}^{}} \right)^{\frac{k-1}{k}} \right\]}$$
where A<sup>\*</sup> is the throat area of the nozzle
(*m**m*<sup>2</sup>), A<sup>*e*</sup> is the exit area of the nozzle
(*m**m*<sup>2</sup>), P<sub>*e*</sub> is the exit pressure (*a**t**m*),
P<sub>*o*</sub> is the chamber pressure (*a**t**m*) and finally *k* is
the ratio of specific heats of the exhaust products.  
  
The loss of performance due to the straight-cut region in the nozzle was
calculated and deemed to be insignificant for the design of this motor
(1 sec. of specific impulse lost for 3 mm throat length)  
  
Sealing will be achieved with two O-Rings.

## Retaining ring - Nozzle

Utilizing the same formulas used for the bulkhead we can calculate that
the groove of the nozzle’s retaining ring needs a load of 17.55 *k**N*
in order to fail, calculating for pressure, the chamber has to reach
14.9 *M**P**a* in order for the retaining ring groove to give in and
break. We can observe that the groove of the nozzle needs 1.6 MPa *more*
pressure in order to fail, that is favorable because the nozzle is
harder to machine than the bulkhead.

# Ignition

For the ignition a simple blackpowder pyrolant will be used placed
inside a drinking straw with a 10 mm section of nichrome
(nickel-chromium) wire. The blackpowder will be packed tightly inside
the straw and then silicone will be used to seal the whole igniter.

## Igniter Amount & Pressure Rise Due to Igniter and Primer

Calculations for the amount of blackpowder used are TBD. The goal is
when the ignition occurs that the ingiter and ignition primer gasses do
not exceed the MEOP of the motor (3.67 MPa)  
I am now calculating the mass per area that the ignition primer can coat
so i can calculate the pressure rise due to the primer to then calculate
how much pressure there is left over for the igniter to finally
calculate the igniter mass.

# Performance Graphs

## Chamber Pressure

<img src="Pressure-Time.png" style="width:50.0%" alt="image" />

## Thrust

<img src="thrust-time.png" style="width:50.0%" alt="image" />

# Drawings & Renders

## Assembly

<img src="assembly render.png" style="width:50.0%" alt="image" />

<img src="assy.png" style="width:50.0%" alt="image" />

## Nozzle

<img src="nozzle-cross.png" style="width:30.0%" alt="image" />

<img src="Nozzle-Render.png" style="width:50.0%" alt="image" />

## Bulkhead

<img src="Bulkhead-cross.png" style="width:50.0%" alt="image" />

<img src="Bulkhead.png" style="width:50.0%" alt="image" />
