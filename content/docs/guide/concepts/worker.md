---
title: Worker
description: Workers complete Tasks
weight: 85
---

## Overview
Persons and Robots are classified as Workers. Workers are responsible for working on [Tasks]({{% relref "task" %}}) and [Missions]({{% relref "mission" %}}).
A Worker can move around a Settlement to do Task, in addition a Person can be EVA Tasks.
All Workers are not equal as they have individual Skills and Attributes that contribute to their effecient and performance.

## Skill
Every Worker has a variety of skills at their disposal and may acquire the following skills at the beginning of or during the simulation. The level of certain Skills contribute towards how a Task is completed.

### Skill Types
Skills can prove useful in various tasks while stationed, and can improve with exercise. Skill proficiency is measured in levels, where Level 0 is the lowest level. 

* `Areology` - the Martian equivalent of geology, areology is the study of the surface, crust, and interior of Mars.
* `Astronomy` - like on Earth, astronomy is the study of celestial objects, the physics, chemistry, mathematics, and evolution of such objects.
* `Biology` - the study of life and living organisms, including their structure, function, growth, evolution, distribution, and taxonomy. On the Mars settlement, this is mostly human focused.
* `Botany` - a branch of biology, botany is the science of plant life.
* `Chemistry` - the study of the composition, properties and behavior of matter.
* `Computing` - the mastery of using devices to perform computation.
* `Construction` - a process that consists of the building or assembling of infrastructure.
* `Cooking` - the art or practice of preparing food for consumption with the use of heat.
* `EVA Operations` - EVA stands for Extra-vehicular Activity and covers all kinds of operations performed outside a habitat or vehicle.
* `Management` - the administrative talent for managing the settlement.
* `Materials Science` - is an interdisciplinary field applying the properties of matter to various areas of science and engineering.
* `Mathematics` - the abstract study of topics such as quantity, structure, space, and change.
* `Mechanics` - the branch of science concerned with the behavior of physical bodies when subjected to forces or displacements, and the subsequent effects of the bodies on their environment.
* `Medicine` - the field of applied science related to the art of healing by diagnosis, treatment, and prevention of disease.
* `Meteorology` - the interdisciplinary scientific study of the atmosphere.
* `Physics` - the study of matter and its motion through space and time, along with related concepts such as energy and force.
* `Piloting` - the controlled operation and movement of a vehicle, such as drones, explorer rovers, transport rovers, cargo rovers, and light utility vehicles.
* `Psychology` - the study of human psyche and the affinity to apply psychological insights in interpersonal relationship.
* `Reporting` - writing reports, capturing the moments and putting together documentary/docudrama. 
* `Trading` - the transfer of the ownership of goods from one person or entity to another by getting something in exchange from the buyer.

The skill level affect the outcome of the task a person perform in terms of *speed* and *efficiency*.

### Multiple Skills 

Although each one of these skills corresponds to a specific [Job]({{% relref "management#jobs" %}}), a Worker is not limited to have one and only skill. e.g. A person may be a `Biologist` and he may have a level 2 `Biology` skill, level 1 `Mechanics` skill, and level 3 `Botany` skill.

### Experience Points

A Worker's skill may advance to the next level by repeatedly performing pertinent tasks to gain experiences so that their experience points may reach the next level threshold. 
The formula for calculating the needed experience points for the next level is `25 * 2^ level`.

### Labor Time 

Labor time is measured in millisols as experienced on Mars. It tracks how much time a Worker spends in performing a Task that makes use of a skill. At the beginning of a new simulation, the labor time of a skill in a Worker always starts at zero. 

Most of the time, a Worker will be less likely to chose a certain task that they lack the skill set to do so. 

### Initial Skill
The set of Skills assigned to a Worker uses an algorithm to ensure not all skills set at zero.

Robot skills are defined by their associated [Robot Spec]({{% relref "/docs/definitions/robot" %}}).

Person skills are created randomly but heavily influenced by their assigned [Job]({{% relref "management#jobs" %}}).

## Attributes
In addition to Skills, Workers also have `National Attributes` which reflect their personality.

