---
title: Mission
description: Missions allow Workers to achieve objecttives
---

## Overview

Missions are outdoor expeditions undertaken by Workers. Normally, the settlement prioritizes what missions to conduct at a given time based on its needs. 

While Missions are generated automatically by mars-sim, user may also create any particular missions manually via the `Mission Tool`.

Also, all ongoing missions are tabulated at the Mission tab in the `Monitor Tool`.

### Mission Types

The 12 types of Missions are as follows : 

| Type of Missions |
| --- |
| Areology Study Field Mission |
| Biology Study Field Mission |
| Building Construction Mission |
| Building Salvage Mission |
| Collect Ice |
| Collect Regolith |
| Delivery |
| Emergency Supply Mission |
| Exploration |
| Mining |
| Rescue Salvage Vehicle |
| Trade |
| Travel To Settlement |

### Mission Phase

A typical mission comprises a few phases as follows : 

| Type of Phases |
| --- |
| Organizing |
| Approving the Mission Plan |
| Embarking |
| Travelling to Next Nav Point |
| (Various Stages depending on the Mission) |
| Disembarking |
 
At the beginning, if the starting member cannot find mission capable personnel or adequate resources, he/she may fail to successfully organize the excursion. 

### Mission Planning Score

Also, during the `Approval` phase, a senior leader such as a commander, sub-commander, or a chief will review the mission plan and provide a composite score that is made up of the following 10 areas : 

| Type of Scores | Description |
|:------ |:--- |
|(1) Rating | mission lead's cumulative job rating |
|(2) Relationship | mission lead's relationship score with the reviewer |
|(3) Qualifications | mission lead's mission qualification |
|(4) Objective | does this mission fit into the settlement's overall objective |
|(5) Emergency | is this a rescue or resupply mission ? |
|(6) Site Value | how accessible or how good are the collection rates are the sites to be visited |
|(7) Distance | how many km is the proposed distance traveled |
|(8) Leadership | how good is the mission lead's ability to lead |		 
|(9) Reviewer Role | the weight of the role of the reviewer. (e.g. The commander as the reviewer has the highest weight) |
|(10) Luck | add a little bit of randomness |

The Mission Plan must be reviewed and scored a few times separately (hopefully by up to 5 different senior leaders). It will combine these scores and compute an average score. If the average score passes a certain threshold value (also known as the passing score), then the Mission is approved.
 
> Note that during each review process, the passing score is being recomputed and is therefore different each time. 



