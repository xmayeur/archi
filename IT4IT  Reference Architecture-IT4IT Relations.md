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

Here lives the CI in the CMDB

### CI (Business Object)

That's the *configuration item*

**Relationships**

|From|Relationship|To|Name|Description|
|---|---|---|---|---|
|CI|Association Relationship|[Incident (Business Object)](#incident-business-object)|[n::n]|Incidents are related to CIs|


**Relationships**

|From|Relationship|To|Name|Description|
|---|---|---|---|---|
|Config Mgt|Access Relationship|[CI (Business Object)](#ci-business-object)|||


## Incident Mgt (Business Function)

How I manage Incident

### Incident (Business Object)

The *Incident* object

**Relationships**

|From|Relationship|To|Name|Description|
|---|---|---|---|---|
|Incident Mgt|Access Relationship|[Incident (Business Object)](#incident-business-object)|||


## Service Discovery (Business Function)

It is the Service Discovery

**Relationships**

|From|Relationship|To|Name|Description|
|---|---|---|---|---|
|Service Discovery|Flow Relationship|[Config Mgt (Business Function)](#config-mgt-business-function)|Actual CI|Discovery feeds the CMDB|



*Generated: Sun Feb 10 2019 13:17:02 GMT+0100 (CET)*
