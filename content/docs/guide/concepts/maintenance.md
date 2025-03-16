---
title: Maintenance
description: Maintenance and Fault Simulation
---

## Overview

Maintenance is predictive in nature. A good maintenance program is when maintenance are scheduled in advance and 
does not wait until something breaks. 

### Inspection vs. Needed Parts
In mars-sim, the inspection portion of maintenance is currently set to get started, say, a quarter of time, into its maintenance window. Inspection means simply taking a close look at the system and parts and will not generate needed parts to be swapped out. 

On the other hand, if a maintenance even does create needed parts, it is a preventative measure to avoid [Malfunctions]({{% relref "/docs/definitions/malfunction" %}}).

### Concept
The concept of maintenance involves a few parameters such as *Wear and Tear*, health condition, time since last inspection/maintenance, number of inspections, etc. Currently, the scope of both maintenance and malfunction modeling are found on the following types of entities: 
 
| Entity|
| --- |
| Building |
| EVA suit |
| Vehicle |

### Wear
First of all, the wear from use over time plays into how likely an entity degrades. The simulation would track the amount of *active use time* for EVA suits, vehicles, and buildings and determines the amount of maintenance needed.

### Needed Parts 
Usually, an engineer or technician will perform maintenance task on an entity that's due for a maintenance task.

If [Needed Parts]({{% relref "/docs/definitions/part" %}}) are involved, they will be pulled from the entity and may be retrofit and put back to work. 
