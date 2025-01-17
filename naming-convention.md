# Naming Convention

This file contains the naming convention used when creating new network resources for ERP.BG 

## Canonic Name
`<location>-<group>-<resource><no>`
  
where:

## Location

Location usually denotes the physical data-center or office, where the equipment is located.
However, internal use VMs are located in a virtual location, called "INT".
PCs, routers and other physical equipment are allocated to a location.

* **BG1** - Physical equipment - Location BG1 = Bulgaria Telepoint Sofia Druzhba
* **INT** - Virtual machines for internal use (office/dev)

## Department

* **ADM** - Administration + Sales + Marketing
* **PD** - Product Design. Previous names: "SUPP", "XP", "BA"
* **DEV** - Development 
* **SYS** - System administration
* **PAR** - For use by partner
* (skipped) - For any host, for which we do not need division by department (for example: DB servers, physical servers, etc.)

## Resource

Indicates the type of the actual resource.
The type of the resource denotes whether the resource is physical or virtual.

Common types of resources are:

* SERVER - physical server (Physical)
* RTR - physical router (Physical)
* VRT - virtual router (VM)
* NET - physical network resource (Physical)
* VNET - virtual network resource (VM)
* VM - generic, unspecified virtual machine (VM)
* PC - physical personal computer - laptop, all-in-one, desktop, etc. (Physical)
* APP - ERP.net application server (VM)
* DB - Database (SQL) server (VM)
* DC - Domain Controller (VM)

## No (number)

The unique number of the specific resource.
Prefer two digits - 01..99.

## Examples

* BG1-SERVER14 - physical server 14 (in BG1 datacenter)
* BG1-SYS-RTR03 - physical router (in BG1 datacenter)
* BG1-SYS-VRT03 - software router (in BG1 datacenter)
* BG1-SYS-DC01 - domain controller (in BG1 datacenter)
* AZ-PD-DB01 - Database server in Azure for the BA department
* INT-PD-DB01 - Virtual database server, PD department
* INT-PD-NBETA - Virtual machine, PD department
* HQ-ADM-PC01 - Personal computer 1 in the Administration department (in the Head office)
* HQ-DEV-PC01 - Personal computer 1 in the Development department (in the Head office)
