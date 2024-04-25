# Zabbix - TL1000/IBM-2900 SNMP Monitoring

The [Dell PowerVault TL1000 Tape Library](https://www.dell.com/en-us/shop/data-storage-and-backup/powervault-tl1000/spd/storage-tl1000/pw_tl1000_11595) is basically a rebranded [IBM TS2900 Tape Autoloader](https://www.ibm.com/products/ts2900) - so this template should work for all devices based on it.

Also: IBM 3572-TL, IBM ULT3580-HH8

----

## Items

* Description
* Location
* Model
* Link Speed
* Uptime
* Drive Firmware
* Library Firmware
* Controller State
* Magazine State
* Controller Status
* Drive Status
* Magazine Status
* Power Status
* Robot Status
* Tapes
* Error-Event Discovery

----

## Triggers

* Controller Status (avg)
* Drive Status (avg)
* Magazine Status (avg)
* Power Status (avg)
* Robot Status (avg)
* Low Uptime (info)
* Firmware Change (info)
* Magazine Open/Unlocked (warn)
* Error-Events

---

## Install

* Import Zabbix Template
* Configure Tape Library as Host with SNMP interface
* Link Template

----

## Extend

SNMP MIBs ca be downloaded:
* [Dell](https://www.dell.com/support/home/en-tc/drivers/driversdetails?driverid=knhyt)
* [IBM](https://www.ibm.com/support/fixcentral) (TS2900)

The whole list of SNMP OIDs can be found here:
* [numeric](https://github.com/NiceRath/zabbix-tl1000-snmp/blob/main/oid-numeric.txt)
* [human-readable](https://github.com/NiceRath/zabbix-tl1000-snmp/blob/main/oid-full.txt)