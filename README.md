# My Home Assistant configuration. 

I've installed HA on an HP mini PC under proxmox. (CPU i3 / 16GB RAM / 500 GB SSD)

You can find out more about me and my smart home installation here: https://homeassistant.com.de/

My HA configuration uses packages, so if you whant to use anything of my configuration, take a look at https://www.home-assistant.io/docs/configuration/packages/.

To use packages, add this lines in your configuration.yaml 
```homeassistant:
  packages: !include_dir_named packages
```
Then copy the yaml files into your preferred sub-structure under \packages.

Files with a suffix similar to .yaml.1 are working copies for me, or older code that I still want to keep. Please ignore these files, or use them very carefully.

Packages splits the configuration, so it is possible to divide by topic, not just by “automation” / “sensor” / “scenes” etc.
I have created a package for each major topic. At the moment the following packages are documented:

| package | Description |
| --- | --- |
| `deye` | deye 8K inverter integration via modbus rtu over tcp |
| `energiedashboard` | my own energydashboard with PV integration |
| `lambda` | Lambda heat pump integration via modbus |
| `mold` | mold sensors for all rooms |

I'll publish my dashdoards later, they are still under construction.
