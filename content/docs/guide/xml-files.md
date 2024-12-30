---
title: Configuring XML Files
linktitle: XML Files
description: Overriding the XML Configurations
weight: 80
---

This guide will get you started with editing the XML files.

Most of the Mars Simulation Project's configuration files are primarily written in XML format. Some are in JSON. 

At the beginning of a sim (whether it is starting a brand new sim, or loading from a new sim), the values/attributes/properties contained in these xml files will be *read* into your local machine's Java VM memory.

Most attributes and properties are designed to tolerate a range of values. However, they are not all created equal to have the same degree of user customization. 

Note that when saving a sim, it will not alter any XML files. 

## Location

At startup, they are being copied into user's home directory. Players may manipulate these XML files in /.mars-sim/xml folder. The file can be editted in this location but changes will be overwritten when a new simulation starts unless the file name is added to the exception.txt file.
 
## Backup

It is recommended that you make a backup of the original xml configuration file before editing them as edited XML files often contain errors that may result in a failure for mars-sim to boot up.

Whenever a new build or version of mars-sim is executed, it will attempt to compare the version content of the `version.txt` file in the `/.mars-sim/xml` folder to determine if it matches the core engine's build version. 

If they don't match, mars-sim will attempt to backup the existing XML files on user home into a new directory inside the `backup` folder. 

## List of XML files

| File name | Description |
|------|-------|
| buildings.xml | Define new buildings with functions |                  
| construction.xml | Define type of foundations, frames and buildings |
| country/country\__name_.xml | Define settler's names for a country |
| crew/crew\__name_.xml | Store a crew roster |
| scenario/scenario\__name_.xml | Define the default settlement scenario |
| settlement/settlement\__name_.xml | Define the building placements for a settlement template phase |
| building_packages.xml | Define building packages for use in settlement templates |
| buildings.xml | Define building placement for use in settlement templates |
| construction.xml | Define a list of foundations, frames and buildings that can be constructed |
| crops.xml | Define food crops grown in greenhouses |
| food_production.xml | Define food technology related processes |
| governance.xml | Define country and sponsor objectives and mission agendas, as well as settlement and rover naming scheme |
| landmarks.xml | Define landmarks on the surface of Mars |  
| malfunctions.xml | Define malfunctions that can occur in the sim |
| manufacturing.xml | Define manufacturing processes  |
| meals.xml | Define main dish and side dish recipes |
| medical.xml | Define illnesses or treatments |
| minerals.xml | Define mineral types |
| part_packages.xml | Define part packages for initial settlements or resupplies from Earth |
| parts.xml | Define parts |
| people.xml | Define properties related to people |
| resource_process.xml | Define resource processes |
| resources.xml | Define resources |
| resupplies.xml | Define initial settlement resupply packages from Earth |
| robots.xml | Define robot types |
| settlements.xml | Define properties related to settlements |   
| simulation.xml | Define simulation properties |
| vehicles.xml | Define properties related to rovers, luvs, and drones |