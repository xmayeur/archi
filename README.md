# Relations

* [Introduction](#introduction)
* [Config Mgt (Business Function)](#config-mgt-business-function)
  * [CI (Business Object)](#ci-business-object)
* [Incident Mgt (Business Function)](#incident-mgt-business-function)
  * [Incident (Business Object)](#incident-business-object)
* [Service Discovery (Business Function)](#service-discovery-business-function)

## Introduction

![Relations][embedView]

## Config Mgt (Business Function)

**Relationships**

|From|Relationship|To|Name|Description|
|---|---|---|---|---|
|Config Mgt|Access Relationship|[CI (Business Object)](#ci-business-object)|||


### CI (Business Object)

**Relationships**

|From|Relationship|To|Name|Description|
|---|---|---|---|---|
|CI|Association Relationship|[Incident (Business Object)](#incident-business-object)|[n::n]||


## Incident Mgt (Business Function)

**Relationships**

|From|Relationship|To|Name|Description|
|---|---|---|---|---|
|Incident Mgt|Access Relationship|[Incident (Business Object)](#incident-business-object)|||


### Incident (Business Object)

## Service Discovery (Business Function)

**Relationships**

|From|Relationship|To|Name|Description|
|---|---|---|---|---|
|Service Discovery|Flow Relationship|[Config Mgt (Business Function)](#config-mgt-business-function)|Actual CI||


[^1]: Generated: Fri Feb 08 2019 22:48:40 GMT+0100 (CET)

[embedView]: README.png