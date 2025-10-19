---
title: Version History
linktitle: Version
description: History of the MarsSim releases
weight: 50
---
## Version 3.10.0 (Oct 2025)

### A. CORE ENGINE IMPROVEMENTS:

- Meal time schedules are flexible and follow the sunrise.
- Different toolsets requirements can be defined for Manufacturing Processes.
- Manufacture function can provide multiple toolings for processes.
- Simplify the start up for the Simulation configuration.
- Default configuration directory can be changed by a commandline argument.
- File logging is controlled from a commandline argument.
- Dessert creation merged into normal Dish/Meal configurations.
- Mission outcome/objectives are held seperate from the Mission class. This support future of mixed purpose Missions.
- Remodel and display a person's blood type.
- Remodel a person's eating appetite.
- Rebalance biomass yield on food crop.
- Add Sector Base Template with population of 120.
- Replace with efficient pathfinding algorithm for settlement interior walk.
- Rework Loading Dock Garage to support 3 bays for rovers.
- Add 2 LUV bays in both garages.
- Add to garage when a vehicle returns to a settlement.
- Add Alpha Base template variants.
- Optimize getting a set of buildings.
- Moderate food resource and food production.
- Lower structural heat loss due to proximity of adjacent building.
- Add bunk beds in some buildings for accommodating more settlers.
- Add Parameter Categories for customizing preferences in each settlement.
- Add Brine Water Well building to lessen the need for digging local ice and ice collection mission.
- Implement construction queue
- Improve inspection and maintenance. Allow auditing outside buildings remotely.
- Create MarsZone, StorageSpec, Research Spec, GenerationSpec and SourceSpec.
- Unify access to walking methods for persons and robots.
- Rework how local construction tasks are executed during a construction mission
- Rework various settlement templates and experiment with new building placements.
- Create and rework coordinate format to be non-locale based in support of internationalization.
- Add more German and UK person, settlement and vehicle names.
- Add Agenzia Spaziale Italiana, German Space Agency (DLR) and UK Space Agency (UKSA).
- Add part fatigues to vehicles, robots and buildings and they may be lowered by inspection and maintenance.
- Limit resource demand with a ceiling imposed by the sum of projected, trade and repair demand.
- Rebalance resources demand and supply chain.
- Add new bio-based and chemical-based resource processes.
- Allow hallways to have sufficient heat capacity by generating heat per square meter of area.
- Add Sociology and Architecture as a science subject.
- Switch to supporting JUnit 5 and 6.
- Rework mission log entries.
- Add the initial model of generating tourists for large settlements.
- Add new background music ogg files.
- Implement new area collision algorithm for walking outside.

### B. UI IMPROVEMENT:

- Person Favorite displays the list of dish names
- Navigator Window provides filters for the Exploration, Unit & Landmark layers
- Redesign of the Navigator Window controls so layers are managed via a Tree control
- Navigator window is no longer a fixed size and can be resized
- Mission details panel redesigned
- New standard way to display Entities with details and location button provided
- Display the average age and gender ratio of a settlement.
- Add 3 dark themes and a light theme.
- Enable top menu bar in macOS.
- Enable mars-sim dock icon in macOS.
- Relocate speed buttons to top left of the main window.
- Add 'Life Core A' and 'Half Core A/B' buildings.
- Add Preferences tab in SettlementUnitWindow.
- Add buildings svg images for new Bio-reactor labs and various Core connectors.
- Improve construction tab with queue table.
- Add deep borehole small drilling site.
- Show spot locations within building in Settlement Map's status bar.
- Fast track building maintenance if repair parts are posted and ready.
- Remove memory leak when scrolling up and down Settlement map's zoom slider.
- Update mass/quantity properly in Monitor Tool's Good tab.
- Add settlement wide construction and manufacturing queue.
- Convert various missions to Objective pattern.
- Reduce heap memory when zooming in the Settlement local Map
- Replace console main menu with a swing-based startup chooser menu
- Allow each tab in Monitor Tool to choose from All, a sponsor or a settlement in authority combobox.
- Add a floating toolbar to host sound control and speed control.

### C. FIXES:

- GoodsManager could use the wrong Good properties when updating the value.
- Correct missing main window title.
- Correct male and female gender ratio.
- Correct the use of Alive/Deceased/Buried checkboxes in Monitor Tool's Citizens tab.
- Correct the use of stock capacity.
- Correct mouse button detection for macOS in Settlement Map.
- Proper artificial lighting for growing crops in greenhouses.
- Correct hatch-facing attribute interpretation for building locations.
- Correct getting a computational node.
- Fix getting a random settlement name.
- Fix calculating local vs. market demand and value points.
- Fix area calculation for hab and hub.
- Fix repairbots getting stuck in EVA airlocks.
- Correct the use of population factor for computing demand and good value.
- Return zero rating for emergency mission.
- Clean up astroart code.
- Update mass/quantity properly in Monitor Tool's Good tab.
- Correct the way the ChainOfCommand elect leaders and chiefs and release old roles.
- Identify and correct teleportation of mission members during mission back to their home settlement.
- Correct the way the power grid would selectively shut down various types of buildings that may generate power to have net position power.
- Correct inability to automatically starting Field Study missions.
- Correct collecting rocks in Exploration and various field missions.

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



## Version 3.8.0 (Aug 2024)

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


## Version 3.7.2  (Feb 2024)

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



## Version 3.7.1 (Jan 2024) 

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



## Version 3.7.0 (Dec 2023) 

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

## Version 3.6.2 (Sep 2023)
 
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

## Version 3.6.1 (Aug 2023) 
### A. FIXES :

- Mineral Map: Avoid NPE after a reload by serializing a list of mineral types 
- <a href="https://github.com/mars-sim/mars-sim/issues/1005">#1005</a>

  
## Version 3.6.0 (Aug 2023) 

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

## 3.5.0 (Apr 2023) 

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


## Version 3.3.0 (Sept 2021)

- Crew Editor : Create and load user-defined crew.
- Equipment : Reduce memory usage - no longer uses Inventory class.
- Authority : Add Authority Editor and allow players to customize sponsors.
- Scenario : Add basic ability to define scenarios. 


## Version 3.2.0 (June 2021)

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


## Version 3.1.1 (July 2020)

- Console: Correct startup issues. Provide a basic way of using CLI to start a single settlement. 
- Goods : refine the conversion between the level of effort of an operation and its modifiers. 
- Commander Dashboard : Correct dashboard's level of effort alignment.


## Version 3.1.0 (Jan 2020)

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


## Version 3.07 (Jan 2015)
- includes new activity spots in buildings and vehicles, improved agriculture and new food production,
new event notification popups, and overall improvements to the UI look & feel.

## Version 3.06 (May 2014)

- adds hallways and hatch connectors between buildings, people walking connected interior paths between buildings and avoiding exterior obstacles
 when walking outside. Internationalization work has started, added German and Danish language text based on the user's locale.


## Version 3.05 (Sept 2013)

- includes a new emergency supply mission, dig local ice task, and a new Debian installation package.


## Version 3.04 (May 2013)

- adds local X,Y locations for people and vehicles in the simulation, vehicles displayed on the settlement map tool, new arriving
settlements can be created/edited with the resupply tool, and a new tutorial window that displays when a new simulation is created (Lars).


## Version 3.03 (Oct 2012)

-  is a maintenance release that focuses on performance improvement, tweaks, and fixing bugs. Includes a new UI start up sound (Lars).


## Version 3.02 (Oct 2012)

-  includes a new resupply tool and adds person labels to the settlement map tool. A large number of bug fixes were made in this release.


## Version 3.01 (Sept 2011)

-  includes improvements on the settlement map tool, two new settlement templates, and seven new buildings.


## Version 3.00 (Jan 2011)

-  has a new simulation configuration dialog that lets the user configure a new simulation, and a settlement map tool that displays a graphical 2D map of each settlement.
Lots of bug fixes and performance improvements.