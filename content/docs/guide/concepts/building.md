---
title: Building
description: Buildings within a Settlement
weight: 40
---
{{% pageinfo color="info" %}}
This is placeholder content.
{{% /pageinfo %}}

## Overview
Buildings provide the physical environment of a Settlement. Each Building can be connection to others or stand-alone. Not all builidngs have LifeSupport features. The Building is defined as providing a set of Functions via a [Building Template]({{% ref "/docs/definitions/building" %}}). 

Each Building also has a Category that summerises the purpose of the Building in the Settlement. This is derived from the most important Function.

Buildings defrade as they are used and therefore need [maintenance]({{% ref "maintenance" %}}) to prevent Faults occurring.

## Physical Characteristics

Buildings can be constructed from a number of materials:
- CONCRETE
- INFLATABLE
- PRE_FABRICATED
- SEMI_ENGINEERED

The type of material contrbiutes to heat loss and how ti survives a meteorite strike. It also has an impact on contriction speed.

## Functions
Each Function has a special purpose and confguration set in the associated building template. Also many have a capacity of how many Workers can use that Function simultaneously.

### Administration
This function provides office space for adminstrative tasks to be completed.

### Algea Farming
This function provides the Building the ability to grow Algea in a farm so that it cna be used as Food.
There is also cleaning activities of the facilities.

### Astronomical Observatory
This function means a Building has the ability to observe the stars. This could be used for social skywatching parties or specialised scientific research.

### Communication
Manages communcation channels to Earth. This function provides a specialised dedicated communcation equipment allowing Persons to contact Earth

### Computation
Represents a dedicated computing resources that can be used generally from throughout the Settlement.

### Cooking
This provides a location where Workers can Cook to create [Meals]({{% ref "/docs/definitions/meal" %}}). This function capacity is aligned to how many hobs/ovens available.

### Dining
This provides an area where Persons can collect to eat Meals together.

### Earth Return
This provides th ablity for Persons to return to Earth via a spacecraft. It is currently under developed in the SImulation.

### EVA
The EVA function provides Airlocks allowing Persons to transfer to the Mars Surface. Airlocks have multiple chambers and usually one Person takes control the of the Airlock process. It includes the wearing and removal of EVA Suits.

### Exercise
A gym used for Persons to complete Exercise related Tasks.

### Farming
Growing of [Crops]({{% ref "/docs/definitions/crop" %}}) is essential to a Settlement and this is provides by this Function. Numerous activities have to be completed continously at this Function to tender the growing crops.

There is also cleaning activities of the facilities.

### Fishery
The Fishery function results in a Building have a pool to support growing Fish. When there is an excess of Fish, a Worker can collect them and use them for cooking.

There is also cleaning activities of the facilities.

### Food & Dessert Preparation
This is complementory to the Cooking function but it is focused on taking raw ingredients and creating food products that can be eaten directly or used in Cooking. There are a number of [Food Recipes]({{% ref "/docs/definitions/food" %}}) that define what produce can be created.

### Life Support
Any Building that support Persons needs to have a Life Support capability. This controls the air mixture. This function will have a capacity limit on the number of Persons that can be supported.

### Living Accomodation
Sleeping quarters for Persons encompasses an allocated bed. Primarily used for the Sleep task.

### Management
Provide office space for the leadership team of a Settlement.

### Manufacture
This function provides a workshop with manufacturing equipment that new inventory to be created or salvaged. Each Workshop has a technical level that contrls what proccesses can e run.
There is a list of configured [Processes]({{% ref "/docs/definitions/process" %}}) defined.

### Medical Care
This provides a SickBay capability that provide [Treatments]({{% ref "/docs/definitions/treatment" %}}) for Persons that suffer a [Complaint]({{% ref "/docs/definitions/complaint" %}})

### Power Generation
This generates power that can be used in the Settlement. The generation will be one of the available sources:
- Areothermal Power Source
- Fission Power Source
- Fuel Power Source, this sources uses a specific resource for fuel.
- Solar Power Source
- Solar Thermal Power Source
- Thermionic Nuclear Power Source
- Wind Power Source 

### Power Storage
Power is critical to the Settlement operations and this Function allows any generated power from Power Generation to be stored for long-term reuse.

### Recreation
This provides an area where Persons can meet out of work. Generally this would be chairs and tables.

### Research
TBD explain features of a Lab
[Research]({{% ref "research" %}})

### Resource Processing

### Robotic Station
This provides a charging station for [Robots]({{% ref "robot" %}}). It can also be used as a parkign area for idle Robots.

### Storage
This covers a storage ability within the Building. Storage can holdany type of [Resources]({{% ref "/docs/definitions/resource" %}}) if there is capacity. Storage can have a capacility limit for particular resources of types.

### Thermal Generation
This provides heat to a Building using one of the supported heat sources:
- Electric Heating Source
- Fuel Heating Source, this sources uses a specific resource for fuel.
- Thermal Nuclear Source
- Solar Heating Source

### Vehicle Maintenance
[Vehicles]({{% ref "vehicle" %}}) need periodic maintenance and this is most easy done when the Vehicle is garaged off the Mars Surface. The function has a garage that can support a fixed number of vehicle spaces. This function can also be used to provide a quicker load/unload process. 

### Waste Processing

## Build a new building

New Building can be constructed by using a Construction Mission. A Building construction generally undergoes 3 stages:
* Foundation
* Frame
* Building

Each stage delivers one of the [Construction Stages]({{% ref "/docs/definitions/construction" %}}).

