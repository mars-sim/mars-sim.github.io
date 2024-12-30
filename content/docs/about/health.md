---
title: Health and Radiation
description: Health and Radiation Modeling
weight: 30
---

mars-sim simulates realistic scenarios in which settler will cope with accidents of all kinds, illnesses, injuries and even death. Each settler has 4 critical health attributes reflecting the person's current physical conditions: Hunger, Fatigue, Stress and Performance level. A person's overall health status may be reported as being well or being sick (such as Suffocating, Recovering from Anxiety Attack/Flu/Pulled Muscle, and Death, etc..)

In version 3.1.0, a radiation exposure modeling based on NASA's studies has been partially implemented to make it realistic. There are 3 possible type of radiation events : (A). The Baseline (B).the Galactic Cosmic Radiation (GCR) (C). Solar Energetic Event (SEP). Each with different level of radiation with SEP the highest level of exposure. The 3 body regions where the exposure are to be tracked are (1) Blood Forming Organ (BFO) (2) Ocular (3) Skin. In our modeling, there are 3 intervals (or counters) for the exposure: (1) 30 days (2) Annual (3) Career. e.g. for BFO, the max limits are set to be 250 mSV for 30 days, 500 mSV for Annual and 1000 mSV for Career.

As a side note here, the Mars rover Curiosity received an average dose of 300 milli-sieverts (mSv) over the 180-day journey. Note that 300 mSv is equivalent to 24 CAT scans, or more than 15x the annual radiation limit for a worker in a nuclear power plant.

One must be reminded that in the forseeable future, Mars is a by-and-large dangerous and unforgiving world. Survival hinges upon how well each settler responds to situations and how well they pull together as a team. Equipment can malfunction and building break down and require maintenance. There are times when one has to go out on a rescue mission to tow a stranded vehicle back to the base.

{{< figure src="/images/insidegreenhouse2.jpg" caption="Working Inside Greenhouse. Image credit: Douglas Shrock-the Artist Shrox" >}}

