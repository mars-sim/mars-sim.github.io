---
title: Settlements
description: Overview of the Settlements
---

## Overview
Settlements are the key entities of a Simulation that drives all interactions and hence are complex with numerous components.

## Settlement Components
A Settlement has many components that, for example, cover Goods and Trade with other Settlements but the ones below provide other entities to simulate.

### Buildings
Buildings make up the location of a Settlement. The Building provide all the Functions to support the Activities of a Settlement and provided an environment for Persons and Robots to exist. Further details can be found in a dedicated page for [Buildings]({{% relref "building" %}}).

### Population
Within a Settlement lives [Persons]({{% relref "person" %}}) and [Robots]({{% relref "robot" %}}). These act  as [Workers]({{% relref "worker" %}}) perform the various Tasks and activities. 

### Appliances/Tools
To perform Tasks the Worker use tools. These can be:
- [Equipment]({{% relref "equipment" %}}) which can be carried by a Worker to help in a Task. 
- [Vehicle]({{% relref "vehicle" %}}) which can carry Workers and Equipment to perform remote Tasks via Missions.

## Resupply Missions
Once established a Settlement can be get regular resupply missions form Earth. The payload of these Missions come from a range of pre-defined [Resupply Manifests]({{% relref "/docs/definitions/manifest" %}}).

## Governance
Governance of a Settlement is controlled at 2 levels.
- Macro level - Control of the objectives of the Settlemetn is defined by a Sponsor in terms of [Reporting Authority]({{% relref "authority" %}})
- Micro level - Individual Persons that run the Settlement follow a [Management Structure]({{% relref "management" %}})

## Definition
A Settlement is a complex entity and it will be created from a Settlement Template. The template defines all the above components.

These can be referenced in the initial Scenario Configuration either directly for current Settlements or future arriving Settlements. The simulation comes with a list of pre-defined [Settlement Templates]({{% relref "/docs/definitions/settlement" %}}).

