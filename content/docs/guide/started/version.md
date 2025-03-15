---
title: Version History
linktitle: Version
description: History of the MarsSim releases
weight: 50
---

## Version 3.9.0 (March 2025)

### A. CORE ENGINE IMPROVEMENTS :

- Help generator expanded to be more flexible.
- Salvage processes & Manufacturing processes consoliddated into single logic.
- Settlements have a single queue to cover all Manufacturing.
- Vehicle Unloading uses a new Status to remove dependency on Vehicle Mission.
- Unit Hierarchy restructured to introduce MobileUnit & FixedUnits.

    
### B. UI IMPROVEMENT :

- Help library expanded to cover all configuration entities.
- New Manufacturing Settlement screen.
- Maps are downloaded asynchronously.
- Reworking of Map Layer logic to increase reuse and reduce computation costs.
  
  
### C. FIXES :

- Resource Process: fix problematic toggle logic.
- Monitor Tool: Displays newly arrived Settlements in Monitor Tool.



## Version 3.8.1 ( Sept2024)

### A. CORE ENGINE IMPROVEMENTS :

- Battery: rework ingredients for making vehicle's battery modules and EVA battery.
- Fertilizer: rework resources for making fertilizers.
- Loading: rework loading/unloading resources independent from vehicle mission.
- Java: update from Java 19 to Java 21.
- Rating: unify how rating score for both mission and task is computed.
- Resource: correct potassium production and related manu processes.

  
### B. UI IMPROVEMENT :

- OpenCL: add a button to turn on/off GPU map loading.
- Surface Map: add rendering shade relief gray maps.
  

### C. FIXES :

- Manufacturing: fix settlement-driven manufacturing and food production.
- Map Zoom: correct seamless zoom level transition when changing from one map to another.
- Salvage: fix salvaging vehicles and equipment.



## Version 3.8.0 (Tue 27 Aug 2024)

### A. CORE ENGINE IMPROVEMENTS :

- Agency: add "International Space Research Alliance" (ISRA), a Chinese-led multi-national alliance and Taiwan nation state.
- Computing: schedule resources of a task from multiple nodes. 
- Country: incorporate Taiwan as nation state.  
- Drone: add modeling thrust and potential energy.  
- Fishery: refine feeding, growing and harvesting fish and weed. 
- Goods Manager: rework relationship with objectives.
- Group Activity: add group activities for a settlement. e.g. birthday parties, council announcements, team meetings etc.
- Health: streamline MedicalConfig, health problem and complaints.
- Heating: revamp heat sink & ventilation.  
- Medical: rework prescribing medication, examining bodies, and recovery tasks.
- Preferences: manage settlement preferences in various categories of mission, 
	    science and task.
- Process Definitions: standardize approach in defining processes such as salvage, 
	    food production and manufacturing.  
- Releases: integrate Gitflow and GitHub Action for building binary releases.
- Resource Process: respond better to toggling resources on-demand. 
- Settlement Tasks: tasks can be selected by On duty & Off duty persons.
- Settlement Template: may define default objective optionally.

  
### B. UI IMPROVEMENT :

- Backlog: add a column showing the task's work scope.
- Building Tab: add tracking heating system parameters.
- Computing: shows heat dissipation, power for load/non-load & cooling demand.  
- Description: display description of all resources, parts, vehicles, buildings, robots.
- Exploration: show types of rocks collected when exploring sites.	
- Health Log: show a person's health history log with complaint types, date started and date cured.
- Monitor Tool: support and filter authorities and settlements in one single combobox.
- Preference: show # active Missions controlled by Preference panel.
- Settlement: add new Process History tab showing all completed Processes.
- Status Bar: correctly show phi and theta of the mouse cursor.
- Vehicle: shows highlighted vehicle box border in settlement map.
  

### C. FIXES :

- Airlock: correctly looks for airlock with least number of occupants.	
- Heating: manage temperature instability via entropy change to 
		  relate temperature change and heat transfer. 
- Launch Date: correct the launch day calculation when it's before 01-Adir-01.
- Navigation: rework vehicle movement to consume fuel and battery power correctly.	
- Parking: set limits in looking for vehicle parking locations recursively.
- Power Generation: correct how power grid turns on/off buildings during 
		  power surplus/deficit.  
- Resource: correct budgeting essential resource on-demand. 
- Resource: resolve dwindling amount of methane and hydrogen.
- Robot Charging: avoid robot battery depletion. Ensure wireless charging 
		  always possible. 
- Salvage Process: Correct problem when scoring the salvage of a vehicle. 


## Version 3.7.2  (Sun 18 Feb 2024)

### A. CORE ENGINE IMPROVEMENTS :

- Amount Resource: rework fertilizer composition to make use of bacteria.
- Construction: revise frame and foundation template.
- Dust Storm: refines log and show occurrences in settlement banner.
- Part: rework use of aerogel tiles for construction mission.
- Resource: remove mortar in ResourceUtil.

  
### B. UI IMPROVEMENT :

- Construction: add new col "Available Material" during construction mission.
- Settlement: correct building overlapping in Hub Base template.
  

### C. FIXES :

- Airlock: add missing airlock to trading outpost and mining outpost template.
- Building: add checking for building collision at startup.
- Greenhouse: correct experience point calculation when tending crops.
- Heating: revise air and water heat sink buffer.
- Power: add missing power set in settlement templates.



## Version 3.7.1 (Wed 17 Jan 2024) 

### A. CORE ENGINE IMPROVEMENTS :

- Building Alignment: add north-south alignment attribute to each building. 
- Building Package: add standalone building sets for faster settlement template creation.  
- Building: add new Syngas Plant building for synthesizing methanol for vehicles.
- Task: add checking for water level change and resource demand in Budget Resource Task.
- Threading: quit clock thread while loop when paused to save CPU cycles.      
- Walking: simplify colision-related methods.    
- Weather: rework refresh timing with 5 weather params.  

  
### B. UI IMPROVEMENT :
 
- Airlock: fix failing to ingress.
- Dust Storm: show dust storm status in settlement map banner.
- ERVs: relocate ERV closer to (0,0) and align next to habs.  
- Layout: rework activity spots and add a lab room in Medical Hab.
- Location Tab: show settlement or vehicle vicinity.
  

### C. FIXES :

- Airlock: avoid getting stuck in pre-breathing phase when a person is too exhausted.
- Goods: ensure no same goods be selected in the buying and selling list.
- Heating: prevent temperature instability and correct air heat ink.
- Heat/Power Generation: correct calculation with methane fuel spent and its power output.
- Maintenance: correct computing maintenance meta tasks and work time.
- Sleep: ensure settler can get some sleep in astronomy observatory.
- Time: limit to certain iterations in A* pathfinding algorithm when walking outside.



## Version 3.7.0 (Thu 28 Dec 2023) 

### A. CORE ENGINE IMPROVEMENTS :

- Activity Spot: spots represent names & reservable spot where Tasks can be completed.
- Algae Pond: add building, function, tasks for growing spirulina. 
- Corporation: add Blue Origin as the 3rd corporation. 
- Country: add UAE and Saudi Arabia.   
- Economy: add GDP and PPP to xml for each country. 
- Group id: rename to com.mars-sim and com.mars_sim in package name. 
- Macro Simulation: simulate lunar colonies with influx of researchers and engineers. 
- Maven: change all maven package names to start with `com.mars-sim`.   
- Person: add average weight & height characteristics per country.   
- Rating: implement rating score for Settlement, Person & Robot Tasks and hold the composite parts of the overall score. 
- Sponsor: add sponsor mode for players to choose in console menu. 
- UnitTests: add more Unit Tests. 

  
### B. UI IMPROVEMENT :

- Monitor Tool: optimize Monitor Model.
- Diplomatic: add diplomatic channel in Command Dashboard for viewing live statistics in Lunar Colonies. 
- Orbit Viewer: zoom in between Mars and Earth's orbit.
- Settlement Map: Reworking fo the map layer logic. Activity Spots are now visible on the map.
- Person Monitor Tool: add tooltip to Task column showing Score breakdown. On Duty indicator on Shift column.
- Robot/Person Activity Panel: redesigned to show the stack of Tasks and alternative Tasks not choosen. Tooltip shows Rating breakdown.
  

### C. FIXES :

- Airlock: avoid getting stuck in pre-breathing phase when a person is too exhausted.
- Conversation: allow settlers to chat with others as a subtask.
- Mars Navigator: ensure each map type remember its previous choice of resolution.
- Mission Table: fix problem with invalid column. 
- Sleep: ensure correct building when assigning a bed.

## Version 3.6.2 (Mon, 18 Sep 2023) 
###  A. CORE ENGINE IMPROVEMENTS :

- Crop: allow changing growing area per crop in Farming.
- Log: remove excessive CPU loads in generating log statements in PowerGrid and ThermalSystem.
- Pending Task: optimize the use of pending task vs. assigning/replacing task directly. 
- Time Ratio: optimize how time ratio increase/decrease can dynamically affect pulse width and TPS in MasterClock.


###  B. UI IMPROVEMENT :

- Crop: use spinner to change growing area for each farm in Agriculture tab in Dashboard.
- Task: display subTask2 and subTaskPhase2 in Activity Tab.
 

###  C. FIXES :

- Computing: rework work time related to consuming computing resources when analyzing map data.
- Digging Local: correct not being able to start digging ice and regolith on its own. 
- Disembarking: optimize and correct how a crew member disembarks vehicle from garage. 
- Equipment: correct transferring container back to settlement after digging regolith/ice.
- Exploration: end EVA if site is not determined. 
- Food Production: correct potato typo.
- Map: correct magnification and zooming issues.
- Settlement: select correctly whether settlers and vehicles are in settlement or its vicinity in Settlement Map.
- Weather: Correct weather param concurrency during reload.

## Version 3.6.1 build 0ac7103 (25 Aug 2023) 
### A. FIXES :

- Mineral Map: Avoid NPE after a reload by serializing a list of mineral types 
- <a href="https://github.com/mars-sim/mars-sim/issues/1005">#1005</a>

  
## 3.6.0 Build 8557 (24 Aug 2023) 

### A. CORE ENGINE IMPROVEMENTS :

- Building    : Add 2 new buildings, namely, Server Farm and Central Hub A. 
- Computing   : Track entropy in each computing node. 
- Country     : Allow each country's names to be loaded on demand. 
- Crop        : Add a new category of herbs. 
- Earth Time  : Model using the standard Java LocalDateTime class.
- Elevation   : Adopt higher resolution height data.  
- EVA Suit    : Refine the modeling of resources needed to produce the suit parts.
- EVA Time    : Add scheduling EVA time to start right after sunrise.
- Fuel        : Enable the use of methanol as fuel for vehicles.
- History     : Add History class to tally time-dependent events.
- Mars Time   : Model using the standard Java LocalDateTime class.
- Mission     : Retains reference to Vehicle after Mission completed.  
- Power       : Model nuclear reactors with more parameters.
- Reliability : Tweak malfunction probability and rework how various factors relate to one another.	
- Resupply    : Define resupply missions with a repeating schedule.
- Resources   : Allow alternate resources for manufacturing and food production.
- Settlement  : Keep track of settlement preference task/mission/science modifiers. 
- Sites       : Discover & estimate mineral concentration of potential sites.
- Training    : Replace hard-coded training-history-to-role mapping with external xml configuration.
- Vehicle     : Enable regen braking and encapsulate propulsion calculations in motor controller class.


### B. UI IMPROVEMENT :

- Connection : Simplify building connection definition with hatch-facing attribute.
- Events     : Events in the Monitor Window are clickable to drill down into the details of the entity.
- Mars Map   : Add zooming capability, add more map types, and allow maps to load various levels of resolutions.
- Mineral    : Optimize mineral layer loading speed in Mars globe Navigator.
- Resupply   : Showcase resupply missions by settlements under a tree.
- Role       : Restore previous role if change is not confirmed.
- Scenario   : Scale up default scenario to including 12 settlements.
- Search     : Add search term history and add equipment list in Search Tool.
- Settlement : Display settlement preference task/mission/science modifiers and allow players to edit scores. 
- Splash     : Add 3 more splash pictures.
- Template   : Add Hub Base settlement template that features a Central Hub at the center of the base. 
- Vehicle    : Retain vehicle reference to completed missions.
- Weather    : Correct weather icon switching in Settlement Map.
  

### C. FIXES :

- EVA Suits  : Ensure EVA suits retain in vehicle during mission.
- Meteorites : Rework what reasonable malfunctions an meteorite impact would trigger.	
- Social     : Avoid concurrency issue by making relationship score updating in one direction.
- Resources  : Correct displaying amount resources stored in Inventory Tab.

## 3.5.0 (build 7907) - 5 Apr 2023 

###  CORE ENGINE IMPROVEMENTS :

-    Battery : Standardize battery capacity. 
-     Events : Supports future scheduled events to better handle periodic actions on the entities.  
-    Mission : Add deadline on rover mission departure. Split embarking phase into loading & departing.  
-      Parts : Add silica aerogel as transparent rooftop tiles.   
-      Robot : Define specifications using RobotSpec class.   
-      Shift : Add shift manager to handle work shift change and add on leave status.  
-  Stock Cap : Increase general/cargo capacities and specific resource storage capacity. 
-    Storage : Allow selection of storage bin in DigLocal task based on building resource capacity. 
-       Task : Define SettlementMetaTask and track a pool of shared tasks.   


###  UI IMPROVEMENT :

-   Desktop : Remember tools' position and contents. 
-       L&F : Look and Feel can be changed via Settings menu item. 
-   Mission : Organize missions under a tree structure for each settlement.   
-    Panels : Separate tables for Maintenance, Waste and Resource processing. 
-   Styling : Single styling via look and feel applied to all components. 
-       Tab : Add new tab to the Monitor Tool to show task backlog of each settlement. 


###  RUNTIME ENVIRONMENT :

- Java : Require Java 17 or above.  


###  FIXES :

-  EVA Suit : Allow suit repair in a vehicle using repair task. 
-  Jar file : Make settlement template name readable by using lowercase letters. 
-     Robot : Correct robot battery status to be based on percentage, instead of actual KWh. 
-   Vehicle : Correct fuel consumption calculation. 


## 3.4.0 (19 Nov 2022)

###  CORE ENGINE IMPROVEMENTS :

-   Base Mass : Add base mass to all buildings, in preparation for calculating overall rocket payload mass. 
-    Building : Add building general info such as dimensions and mass. 
-   Computing : Add computing function and skill. Track computing resource usage. 
-      Filter : New Settlement filter and Building tab to the Monitor Tool. 
-   Inventory : Replace with lightweight inventory for all units. Revamp the storage of resources/equipment and transfer of person/vehicle between locales.
- Malfunction : Tidy up malfunction and maintenance logic on vehicles, buildings and equipment.
-     Mission : Restructure and simplify handling of Mission.
-       Parts : Add garment and thermal bottle. 
-      Person : Track exercise. Make a person's carrying capacity to be age-dependent.
-  Processing : Unify resource and waste processes, food production and manufacturing under common super class.  
-       Robot : Track battery capacity and charging.
-     Trading : Compute and relate the cost, profit, and price of trade goods.
-    Scenario : Configure arriving future Settlements from a scenario. Scenarios can be exported and shared. 
-        Site : Explore, claim and track mining sites.
-      Social : Remove global relationship graph and simplify codes.
-    Sunlight : Predict sunrise and sunset at each settlement. Track actual sunrise and sunset time.
-   Meta Task : Implement TaskJob approach and remove duplicate computation of outstanding tasks.
-     Vehicle : Rework vehicle specifications. Refine fuel economy calculation.

  
###  UI IMPROVEMENT :

-   Authority : Add editor that customize sponsors/authorities. 
-       Chart : Auto select bar and pie chart.
-    Economic : Display the cost/profit/price of a good in each settlement for comparison.
-       Icons : Replace word title of each tab with an icon in all Unit Windows.
-    Location : Show areocentric longitude of Mars in Time Tool.   
-       Power : Display generated/load power & stored energy for settlements in Monitor Tool.
-    Scenario : Edit and load basic scenarios.
-      Window : Add new Building Window with tab, replacing old Building tab.
  

###  FIXES :

-     Airlock : Fix bugs during EVA egress and ingress. 
-    Delivery : Resolve stalled negotiation. 
- Exploration : Revisit existing sites until they reach an evaluation ready for Mining. 
- Maintenance :	Ground vehicle maintenance no longer stalls when EVA is aborted. 
-     Mission : Fix the mission selection. Correct Navigation tab.
-  Settlement : Correct settlement selection in Monitor Tool. 
-     Trading : Consider loading/unloading edge cases for Trading/Delivery. 
-   Transport : Correct handling of arriving settlement by transport manager.  
-     Vehicle : Correct vehicle fuel calculation.


## Version 3.3.0 (09/25/2021)

- Crew Editor : Create and load user-defined crew.
- Equipment : Reduce memory usage - no longer uses Inventory class.
- Authority : Add Authority Editor and allow players to customize sponsors.
- Scenario : Add basic ability to define scenarios. 


## Version 3.2.0 (07/06/2021)

- Sleep : Enforce one continuous sleep session as much as possible.
- EVA : Remove the duplicated EVA function in garages. 
- Collect Ice : Refine ice collection rate. Higher above +60 deg latitude and below -60 deg latitude.
- Site Score : Compute score for collecting ice/regolith, mineral exploration, and mining.
- Job : Add new job 'psychologist' and new skill/science type 'psychology'.
- Crew Editor : Add saving/loading beta crew. Add choosing destination for each crewman. 
- Job : Adjust job prospect. Refine job assignment for each settlement.
- Work Shift : Designate the name (e.g. Night, Day, and Swing shift) for XYZ work shift. Designate the name (e.g. Day and Night shift) for the AB work shift. Change the start and end time for work shift A (Day shift) and work shift B (Night shift).
- Skill : Add teaching reward and learning points on skills when performing Teach task.
- Task : Report to mission control. Make a reading task contribute to adding experience points to a skill.
- Country : Add settlement and vehicle names tailored to its sponsor/country.
- Airlock : Revamp EVA egress and ingress phases to model airlock activities in finer details.
- Icon : Incorporate Weblaf's IconManager for caching svg icons.
- Science : Add 'Engineering' and 'Psychology' as a new science subject.
- Weather : Record the values of solar irradiance at each settlement.
- XML : Auto-sense user-edited xml files and back them up when checksum are mismatched. Allow a list of exception xml files.
- Threading : Logically partition the calling of units by settlement.
- Clock : Revamp sending time pulse and clock threading.
- Mind : Rework acquiring new tasks and remove recursive calls inside Mind.
- Console : Refactor console-related class.
- Fishery : Activate the fish farm and enable eating fish.
- Mission : Add delivery drones for carrying cargo between settlements. 


## Version 3.1.1 (07/22/2020)

- Console: Correct startup issues. Provide a basic way of using CLI to start a single settlement. 
- Goods : refine the conversion between the level of effort of an operation and its modifiers. 
- Commander Dashboard : Correct dashboard's level of effort alignment.


## Version 3.1.0 (01/28/2020)

- Role : assigns each person a role to function.
- Leadership Hierarchy : establishes a chain of command in each settlement.
- Robots : assists settlers in performing certain routine tasks.
- Greenhouse operations : revamps crop growth model with unique growth phases for each crop category
- Settlement Objective : selects the development goal for each settlement.
- Weather Panel : keeps track of outside weather data, dust storm formation, etc..
- Radiation Exposure : sets and displays radiation exposure for each person, radiation sicknesses.
- Meteorite Impact : Calculates probability of impacts.
- Achievement : computes the science, social, score for each settlement.
- Job Reassignment : records the change of job assignment.
- Task History : records what a settler does on each sol.
- Sponsorship : shows the main space agency that sponsors a settlement.
- Country of Origin : provides each settler name (first and last name) based on his/her nationality.
- Chat Box : Allows limited ability for querying the settlements and interacting with the settlers. 
- Speed Bar : allows convenient access to speed up, slow down, pause and resume the simulation. 
- Mission Planning : Expands how a mission is conducted. Requires commander approval for each excursion. 
- Sleep Hour : Tracks and records a settler's sleep time on each sol. 
- Emotion : Implements basic emotion using two dimensional array. 
- Logging : Allow players to customize desired logging level. 
- Death : creates a death report on a deceased person. 
- Grid Battery : Improves grid battery charging/discharging model. 
- Dust Storm : Adds dust storm modeling and connects it to wind speed. 
- Heat Modeling : Computes heat gain and loss in each building. 
- Power Modeling : Displays power generated and consumed for each building. 
- Gas Composition : Tracks and monitor each type of gases in each building. 
- Add new background music tracks. 
- Water Extraction : Uses NASA Water Studies to model water extraction from minerals found in regolith. 
- Private Quarters : Designates a specific bed for each settler. 
- Reliability Modeling : Tracks the frequency of part/equipment malfunctions and computes MTBF scores. 
- Science Topics : Adds topics for each scientific study. 
- Meal and Dessert : Adds meal and dessert preparation in each canteeen. 
- Preferences and Favorites : Adds task preferences and favorites for each settler. 
- Energy Level : Adds energy level [kJ] as a health metric for each settler. 
- Vehicle Modeling : Adds fuel cell, drivetrain characteristics, fuel consumption/mileage for each rover. 
- Vehicle Log : Tracks the history of vehicle status change. 
- Map : Adds geological map to Mars Navigator. 
- Commander Dashboard : Adds interactive features and controls in Command Mode. 


## Version 3.07 (01/17/2015)
- includes new activity spots in buildings and vehicles, improved agriculture and new food production,
new event notification popups, and overall improvements to the UI look & feel.

## Version 3.06 (05/12/2014)

- adds hallways and hatch connectors between buildings, people walking connected interior paths between buildings and avoiding exterior obstacles
 when walking outside. Internationalization work has started, added German and Danish language text based on the user's locale.


## Version 3.05 (09/14/2013)

- includes a new emergency supply mission, dig local ice task, and a new Debian installation package.


## Version 3.04 (05/13/2013)

- adds local X,Y locations for people and vehicles in the simulation, vehicles displayed on the settlement map tool, new arriving
settlements can be created/edited with the resupply tool, and a new tutorial window that displays when a new simulation is created (Lars).


## Version 3.03 (10/29/2012)

-  is a maintenance release that focuses on performance improvement, tweaks, and fixing bugs. Includes a new UI start up sound (Lars).


## Version 3.02 (06/10/2012)

-  includes a new resupply tool and adds person labels to the settlement map tool. A large number of bug fixes were made in this release.


## Version 3.01 (09/26/2011)

-  includes improvements on the settlement map tool, two new settlement templates, and seven new buildings.


## Version 3.00 (04/07/2011)

-  has a new simulation configuration dialog that lets the user configure a new simulation, and a settlement map tool that displays a graphical 2D map of each settlement.
Lots of bug fixes and performance improvements.


## Version 2.90 (07/01/2010)

-  includes salvage of equipment, vehicles, and buildings as well as using the Nimbus look & feel (Lars).


## Version 2.88 (01/11/2010)

-  has a new webstart release (Christian), we converted the build environment to a Maven project (Christian), and fixed some bugs.


## Version 2.87 (11/24/2009)

-  includes new science skills, new scientist jobs, a new scientific study
system with related tasks and missions, a new astronomy observatory building (Sebastien), settler
age (Lars), and a new preferences tool (Lars).


## Version 2.86 (05/27/2009)

-  includes XML DTDs, switch to JDom library (Sebastien), rover obstacle
avoidance improvements, trading improvements, fixes for settlement overpopulation, and lots of
bug/performance fixes.


## Version 2.85 (01/26/2009)

-  adds settlement building construction, fuel power generation (Sebastien),
power storage buildings, and a new splash screen sound (Lars).


## Version 2.84 (06/25/2008)

-  includes a mining mission, mineral concentrations, a light utility vehicle
(Sebastien) and an inline user guide (Lars).


## Version 2.83 (03/02/2008)

-  includes manufacturing processes, compressed sound support (Sebastien) and
logging (Sebastien).


## Version 2.82 (11/30/2007)

-  includes repair/maintenance parts, automatic UI settings loading/saving,
and bug/performances fixes.


## Version 2.81 (09/16/2007)

-  includes a new trade mission, credit system and goods valuing system.


## Version 2.80 (03/30/2007)

-  includes a new mission tool for creating, editing and viewing missions.


## Version 2.79 (07/23/2006)

-  includes rover rescue/salvage missions, resources containers, and lots
of bug fixes, refactoring and performance improvements.


## Version 2.78 (10/22/2005)

-  add UI sounds (w/ Dima Stephanchuk), individual person configuration,
cooking task, chef profession, mission and task refactoring, and lots of bug fixes and small
improvements.


## Version 2.77 (10/03/2004)

-  adds EVA suit tear malfunction (Rik Declercq), frost bite/nip illnesses
(Rik Declercq), anxiety attack illness (Rik Declercq), teaching skills, settlement EVA maintenance,
settler gender, settler social relationships (w/ Paul Speed), settler MBTI personalities (w/ Paula
Jenkins), sound support (Dima Stephanchuk), Alpha Base settlement template, lots of bug fixes and
small improvements.


## Version 2.76 (08/04/2004)

-  adds settler stress level, settlement and building crowding, landmark display
(Dalen Kruse), settler job specialities, medical and botany science research, and settlement resupply
missions.


## Version 2.75 (04/15/2004)

-  adds configurable settlement buildings, settlement power grid, resource processes,
ice prospecting mission, historical events in the monitor tool (Barry Evans), vehicle trails and improved
configuration files.


## Version 2.74 (05/21/2002)

-  adds a medical system (Barry Evans) and a malfunction/maintenance/repair system
that allows settlers to die as a result of an illness or accident.  A general inventory system has been
added along with EVA operations as a part of missions or repair.  The Monitor tool has been updated to
allow custom tabs and real-time charts and graphs.


## Version 2.73 (12/27/2001)

-  adds the ability to save and load simulations (Barry Evans).  XML configuration
files allow the user to set simulation properties.  A new Monitor Tool shows a table of units and their
information (Barry Evans).  Many bugs have been fixed (Dalen Kruse).


## Version 2.72 (08/18/2001)

-  includes a Martian timekeeping system (clock/calendar), orbital tracking and
day/night tracking.  The settler AI is completely refactored and includes support for missions.  Two
missions are included: Travel to Settlement mission and Collect Rock Samples Mission.  Sleeping and
eating meal tasks have also been added.


## Version 2.71 (01/31/2001)

-  is primarily focused on refactoring the code and reorganizing the directory
structure.  The simulation and the user interface are now cleanly broken apart into two packages.
Greg Whelan added a new USGS mode that allows 8x zoom on the Mars Navigator surface map with an Internet
connection.  Resources are produced and consumed a great deal more in the simulation.  INSITU resource
processors have been added to the settlements to generate oxygen, fuel and water.
##The problematic Installer application has been removed, but the download for the project is much larger now.


## Version 2.7 (09/08/2000)

-  includes random mechanical failures for vehicles, periodic vehicle maintenance in
settlement garages, and a mechanic task and skill.  The crew of a rover that gets stuck will now slowly
winch it along until it's free again.  Fuel is tracked in vehicles.  Configuration text files are included
so that the user can modify the names of people, settlements and rovers.  The Martian globe in the Mars
Navigator tool renders much faster now.


##05/25/2000 - Version 2.65

-  concentrates on fleshing out settlements and improving the look and feel of the
application.  Facilities were added to settlements, including working greenhouses.  The project now has
a centered logo and a tiled background on its desktop, along with a splash screen at startup.  The toolbar
has been broken up into tool and unit toolbars.  A new tool, the "Search Tool", has been added to improve
searching for units.  A "Tend Greenhouse" task has been added.


##03/04/2000 - Version 2.6

-  provides more functionality for people in the simulation and displays the new
information in a larger person detail window.  People now have natural attributes, skills and tasks.
The basic infrastructure for tasks are in place, but only two tasks, relaxing and driving, are currently
implemented.  Skills are fully implemented, but only one skill, "Driving", is currently used in conjunction
with the driving task.  Natural attributes are fully implemented with many attributes, but only one,
"Experience Aptitude", has current practical use in conjunction with the driving task.
There have been some significant structure changes in the program and all classes have some additional
documentation.


##09/06/1999 - Version 2.5

-  adds obstacle avoidance for rovers so they can go around rough terrain to avoid
getting stuck.  They can still get stuck in really bad terrain, but they generally do better than they used
to.  People also tend to drive to closer settlements now.  Many bugs are fixed and there are a lot of
internal changes that are transparent to the user but should make adding new features later easier.  Rovers
also have designated drivers, rather than just a list of passengers.  Link buttons have been added to unit
dialogs that will open up new unit windows.  A "center map" button has also been added to each unit dialog
to center the navigational window on the unit.  The install application has been modified to use less memory.
More people have been added, some with made up names.


##07/19/1999 - Version 2.4

- replaces the old topographical map with a new one based on recently released
Mars Global Surveyor data.  It is a lot more accurate as the previous one was based on Viking orbiter data,
but doesn't compress as well.  I ended up with a download of 2.05Mb up from 1.6Mb in the last version.
It has a new color legend and the rovers have been calibrated to the new scheme.  I came up with some sample
names for settlements and some of my friends and family have agreed to let me use their names for sample
people.  The code has been cleaned up some as well.  The undistorted original large data files are available
on the site if anyone cares to download them.  They have a slightly better image quality than the install data
files.


##06/30/1999 - Version 2.3

-  has the entire interface redone in Swing.  There's now a desktop to contain
the simulation with a flexible toolbar.  All interface windows have been heavily redone.  The source
code has been cleaned up quite a bit as well.  I've copyrighted the project under the GNU Public License
to assure it remains free and cannot be used as a part of a proprietary project.  The sample people and
settlements from Kim Stanley Robinson's novel, 'Red Mars', have been removed to avoid copyright problems,
and has been replaced by random settlements and all units have simple names for now.


##05/11/1999 - Version 2.2

-  includes an installation application and compressed data files, resulting
in a much smaller download (1.6Mb compared to 6.5Mb).  Both a new Swing and an older command line
version of the installer are included.  You have to run one of the installers to decompress the data
files, but I think the download time saved is worth it.  The data files are slightly degraded due to
the compression, but still acceptable.  I also improved the vehicle terrain grade effect on ground vehicles.
The source code is freely available in a separate download.  I've included a README file with
instructions for installing and running the program.


## Version 2.1 (02/15/1999)

-  includes terrain elevation and average grade effect on vehicles, as
well as some major changes in the vehicle info dialog window.  I have also included the source
code with the full installation.


## Version 2.0 (11/23/1998)

-  includes a sample group of people, (based on some of the First One
Hundred in Kim Stanley Robinson's novel, 'Red Mars') randomly distributed among the settlements,
as well as 15 vehicles.  People, vehicles, and settlements have behaviors and can take action,
and the navigation interface updates every couple of seconds to reflect positioning changes.
Only the most basic actions are currently built in, but the foundation is layed for more
advanced behaviors later.  Settlements, vehicles, and people each have a pop-up dialog window
that displays their information and updates itself.


## Version 1.3 (10/20/1998)

-  includes a sample group of settlements (based on Kim Stanley Robinson's
novel, 'Green Mars'.)  Also added distance legend.


## Version 1.2 (10/06/1998)

-  incorporates a topographical mode to show elevation.


## Version 1.1 (09/28/1998)

-  allows the user to recenter on any point on the map by clicking on it.
I also used double buffering to reduce flash on both the map and the globe.


## Version 1.0 (09/21/1998)

-  is the basic navigation interface.  The interface produces a 300x300
pixel map centered anywhere on the surface of Mars with a resolution of approximately 7.4Km
per pixel edge.


