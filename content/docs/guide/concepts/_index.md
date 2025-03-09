---
title: Simulation Concepts
description: Overview of the concepts
weight: 1
---
The MarsSim project is an autonomous simulation of life on Mars for Settlers living in Settlements.  
Any Simulation is defined by a [Scenario]({{% relref "#scenarios" %}}) that defines the starting conditions.

## Entities

The simulation involves managing many entities and simulating the impact of time on each of them. There are different Entities from the large Settlement down to a small EVASuit. The impact of time affects each type differently and has consequences on other Entities.

Time is simulated as a time pulse that applies a time duration to all entities, the frequency and duratino of these pulses can be altered by the end-user to drive a slower or faster simulation.

## Scenarios
The Scenario provides the starting condition of a Simulation.
The default installation provide a number of predefined [Scenarios]({{% relref "/docs/definitions/scenario" %}}) as well as the ability for a user to create their own can be created via the Scenario Editor tool.
Each Scenario consists of 2 elements of information that the Simulation uses to build the initial set of entities; one for the exiting Settlements and the other future Settlements.

### Existing Settlements

[Settlements]({{% relref "settlement" %}}) are the cornerstone of the Simulation as they are the main modelled entity. Each settlement that exist in the Scenario is defined as:

- A unique name
- A Settlement Template that specifies the physical layout of the Settlement.
- Location on Mars Surface
- The owning Authority
- Population sizes
- Optional Crew. If a crew is present; it's members will be seeded into the initial Settlement population. There are a number of pre-defined [Crews]({{% relref "/docs/definitions/crew" %}}); in addition new Crews can be created via the Scenario Editor.

### Arriving Settlement Mission

This defines any new Settlements that will be created in the future via a Resupply Mission. Currently there is no limit of the size of the supply mission, e.g. a 20 Building Settlement could arrive in one delivery.
The Resupply stipulates all the existing Settlement details with the additino of the future arrival in terms of Sols.

## Activities

The daily life of Settlers and Robots are simulated at a micro level allowing them to perform Activities that may improve the settlements:
- [Tasks]({{% relref "task" %}}) which are activities for an individual to perform.
- [Missions]({{% relref "mission" %}}) these use a group of Settlers to work together to achieve an objective.


