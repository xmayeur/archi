# IT4IT Relations

* [Introduction](#introduction)
* [Config Mgt (Business Function)](#config-mgt-business-function)
  * [CI (Business Object)](#ci-business-object)
* [Incident Mgt (Business Function)](#incident-mgt-business-function)
  * [Incident (Business Object)](#incident-business-object)
* [Service Discovery (Business Function)](#service-discovery-business-function)

## Introduction

![IT4IT Relations](IT4IT%20%20Reference%20Architecture-IT4IT%20Relations.png)

I will describe all relations here


## Config Mgt (Business Function)

**Relationships**

|From|Relationship|To|Name|Description|
|---|---|---|---|---|
|Config Mgt|Access Relationship|[CI (Business Object)](#ci-business-object)|||


Here lives the CI in the CMDB

### CI (Business Object)

**Relationships**

|From|Relationship|To|Name|Description|
|---|---|---|---|---|
|CI|Association Relationship|[Incident (Business Object)](#incident-business-object)|[n::n]|Incidents are related to CIs|


That's the configuration item

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
|Service Discovery|Flow Relationship|[Config Mgt (Business Function)](#config-mgt-business-function)|Actual CI|Discovery feeds the CMDB|


[^1]: Generated: Sat Feb 09 2019 22:27:36 GMT+0100 (CET)
