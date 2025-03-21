---
title: Resource Process - Grey Water Processor
linkTitle: Grey Water Processor
toc_hide: true
hide_summary: true
---
<!-- This is generated by the MarsSim HelpGenertor, do not edit. -->

## Characteristics

| Attribute      | Value |
|--------:|:------|
|Process Time:|200 millisols|
|Work Time:|10 millisols|
|Power Required:|0.32 kW/hr|
|Start On:|false|

## Inputs
| Name      | Input Rate (kg/sol) | Minimum kg | Ambient |
|--------:|:------|-----:|:----|
|[Grey water](/docs/definitions/resource/grey-water)|40.0|0.002|false|
|[Chlorine](/docs/definitions/resource/chlorine)|1.0E-5|0.0|false|

Ambient inputs are consumed from the environment.

## Outputs
| Name      | Output Rate (kg/sol) | Waste Output |
|--------:|:------|-----:|:----|
|[Nitrogen](/docs/definitions/resource/nitrogen)|0.2|false|
|[Nitrate](/docs/definitions/resource/nitrate)|0.2|false|
|[Nitrite](/docs/definitions/resource/nitrite)|0.2|false|
|[Phosphorus](/docs/definitions/resource/phosphorus)|0.2|false|
|[Water](/docs/definitions/resource/water)|39.0|false|
|[Ammonia](/docs/definitions/resource/ammonia)|0.2|false|

Waste outputs are released into the environment and do not need to be stored.


{{< definition-tail version="3.9.0" generatedOn="2025-03-08T21:34:45.1684317" >}}



