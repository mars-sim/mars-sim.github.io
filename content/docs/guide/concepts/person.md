---
title: Person
description: Human Settlers on Mars
weight: 60
---

## Overview
Persons are simulated as autonomous beings that will self manage their time in the simulation. They act as a [Worker]({{% relref "worker" %}}) to complete Tasks.

A Person will also participant in the [Management]({{% relref "management" %}}) of the Settlement by having Job and Roles. Their Job/Role will influence the activities they perform.

## Physical Charactertics
Basic physical charactertics of a Person are modelled in the simulation and change as Persons do activities:
- Fatigue
- Thrist
- Hunger
- Stress
- Personality using Myers-Briggs Type Indicator (MBTI)
- Height, Weight & Age

## Health

Person can suffer health [Complaints]({{% relref "/docs/definitions/complaint" %}}) either caused by accident or illness. Complaints need [Treatments]({{% relref "/docs/definitions/treatment" %}}) for recovery or to prevent escalation into more serious Complaints. 

## Radiation Events
Person's health can be directly affected by radiation. There are three types of radiation events tracked by mars-sim : 

| Type of Radiation |
| --- |
| Solar Energetic Particles (SEP) |
| Galactic Cosmic Rays (GCR) | 
| Baseline Radiation |

The solar wind is a stream of particles, mainly protons and electrons, flowing from the sun's atmosphere at a speed of about one million miles per hour. 
	
Meanwhile, Solar Energetic Particles (SEP) are tangible energetic outbursts at the Sun. They include Solar Particle Events as well as Coronal Mass Ejections.

Galactic Cosmic Rays (or GCRs) are high-energy particles that originate outside of our Solar System. These particles include protons, anti-protons, electrons, positrons and positively charged atomic nuclei whose ultimate origin is unknown to us. 

Baseline radiation is defined as the effect of the solar wind interacting with the surface of a planetary body. Thus it is a *secondary* radiation. 

### EVA Operation 
The Baseline Radiation is being the standard dose of background radiation received during an EVA operation on the surface of Mars.

In a GCR event, EVA operations will be kept minimal but are not necessarily stopped.

In a SEP event, EVA operations will cease (unless the repairs are critical for the survival of the settlement) in order to reduce the exposure of the high dose of radiation exposure. 

We calculate the probability of exposure based on NASA recent studies on Curiosity's Radiation Assessment Detector (RAD).

### Body Region Exposure

There are 3 regions of exposures on a human body that we are interested in examining : 

| Region of Exposures | 
| --- |
| Blood Forming Organ (BFO) | 
| Ocular Lens | 
| Skin | 

For assessment, teh simulation keep track of the exposure over the following 3 time interval :

| Exposure Interval |
| --- |
| 30-Day |
| Annual |
| Career |

The exposure level is in the unit of milli-Sieverts [milli-Sv].


