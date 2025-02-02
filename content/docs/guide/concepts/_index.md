---
title: Simulation Concepts
description: Overview of the concepts
weight: 1
---
{{% pageinfo color="info" %}}
This is placeholder content.
{{% /pageinfo %}}

The Simulation is driven by a [Scenario]({{% ref "#scenarios" %}}) that defines the starting conditions of a Simulation.

## Entities
Time Base Simulation

Event event based

## Scenarios
The Scenario provides the starting condition of a Simulation.
The default installation provide a number of predefined [Scenarios]({{% ref "/docs/definitions/scenario" %}}) as well as the ability for a user to create their own can be created via the Scenario Editor
Each Scenario consists of 2 elements of information that the Simulation uses to build the initial set of entities; one for the exiting Settlements and the other future Settlements.

### Settlements

[Settlements]({{% ref "settlement" %}}) are the cornerstone of the Simulation as they are the main modelled entity. Each settlement that exist in the Scenario is defined as:

- A unique name
- A Settlement Template that specifies the physical layout of the Settlement.
- Location on Mars Surface
- The owning Authority
- Population sizes
- Optional Crew. If a crew is present; it's members will be seeded into the initial Settlement population. There are a number of pre-defined [Crews]({{% ref "/docs/definitions/crew" %}}); in addition new Crews can be created via the Scenario Editor.


### Arriving Settlement Mission

This defines if any new Settlements will be created in the future via a Resupply Mission. Currently there is no limit of the size of the supply mission, e.g. a 20 Building Settlement could arrive in one delivery.
The Resupply stipulates all the existing Settlement details with the additino of the future arrivla in terms of Sols.

## Activities

[Missions]({{% ref "mission" %}})


