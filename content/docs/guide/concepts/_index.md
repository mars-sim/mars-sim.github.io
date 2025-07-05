---
title: Simulation Concepts
description: Overview of the Concepts
weight: 1
---
The Mars-Sim project is an autonomous simulation of human beings living on permanent Martian settlements.  
A simulation can be constructed as a [Scenario]({{% relref "#scenarios" %}}) that defines the initial conditions.

## Entities

The simulation involves managing many entities and simulating the impact of time on each of them. There are different Entities from the large Settlement down to a small EVASuit. The impact of time affects each type differently and has consequences on other Entities.

Time is simulated as a time pulse that applies a time duration to all entities, the frequency and duratino of these pulses can be altered by the end-user to drive a slower or faster simulation.

## Scenarios
The Scenario provides the starting condition of a simulation.
The default installation provide a number of predefined [Scenarios]({{% relref "/docs/definitions/scenario" %}}) as well as the ability for a user to create their own can be created via the Scenario Editor tool.
Each scenario consists of 2 elements that the simulation uses to build an initial set of entities; one for exiting settlements and the other future settlements.

### Existing Settlements

[Settlements]({{% relref "settlement" %}}) are the cornerstone of the simulation as they are the main modelled entity. Each settlement that exist in the Scenario is defined as:

- A unique name
- A settlement Template that specifies the physical layout of the settlement.
- Location on Mars Surface
- The owning Authority
- Population sizes
- Optional Crew. If a crew is present; it's members will be seeded into the initial Settlement population. There are a number of pre-defined [Crews]({{% relref "/docs/definitions/crew" %}}); in addition new Crews can be created via the Scenario Editor.

### Arriving Settlement Missions

New settlements can be created in the future via a Resupply Mission. 
A Resupply Mission may also stipulates specific resources needed for an existing settlement. 
Currently, there is no limit to the size of a Resupply Mission, e.g. a total of 20 new buildings could arrive in one resupply delivery.

## Activities

The daily life of settlers and robots are simulated at a micro level allowing them to perform activities that sustain their settlement:
- [Tasks]({{% relref "task" %}}) which are activities for an individual to perform.
- [Missions]({{% relref "mission" %}}) these use a group of settlers to work together to achieve an objective.


