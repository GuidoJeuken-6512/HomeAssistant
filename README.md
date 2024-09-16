# My Home Assistant configuration. 

I've installed HA on an HP mini PC under proxmox. (CPU i3 / 16GB RAM / 500 GB SSD)
My HA configuration uses packages, so if you whant to use anything of my configuration, take a look at https://www.home-assistant.io/docs/configuration/packages/.

Packages splits the configuration, so it is possible to divide by topic, not just by “automation” / “sensor” / “scenes” etc.
I have created a package for each major topic. At the moment the following packages are documented:

| package | Description |
| --- | --- |
| `deye` | deye 8K inverter integration via modbus rtu over tcp |
| `energiedashboard` | my own energydashboard with PV integration |
| `lambda` | Lambda heat pump integration via modbus |
