# SimpleAddon for SimpleAF
SimpleAddon adds a few extra helpful options for SimpleAF. Included addons are listed bellow

Probe calibration - Dialog window for easier probe setup for probes.
Extras - Stand alone addon options for various extra features.




# Install
SSH into your printer and copy and run the command that matches your probe.



# SimpleAddon for BTT Eddy

```
mkdir -p /usr/data/printer_data/config/SimpleAddon
wget -O /usr/data/printer_data/config/SimpleAddon/eddycalibrate.cfg https://raw.githubusercontent.com/ZeroDotCMD/SimpleAddon/main/SimpleAddon/eddycalibrate.cfg
wget -O /usr/data/printer_data/config/SimpleAddon/quickstart.cfg https://raw.githubusercontent.com/ZeroDotCMD/SimpleAddon/main/SimpleAddon/quickstart.cfg
/usr/data/pellcorp/k1/config-helper.py --add-include "SimpleAddon/quickstart.cfg"
/usr/data/pellcorp/k1/config-helper.py --add-include "SimpleAddon/eddycalibrate.cfg"
```

<br><br><br><br>

# SimpleAddon Extras
This section contains no probe calibrations. Simply the additional scripts and stand alone versions without adding any probe features.


# Quick Start
Quick Start - Automate basic printer calibration such as PID calibration and Input Shaping

```
mkdir -p /usr/data/printer_data/config/SimpleAddon
wget -O /usr/data/printer_data/config/SimpleAddon/quickstart.cfg https://raw.githubusercontent.com/ZeroDotCMD/SimpleAddon/main/SimpleAddon/quickstart.cfg
/usr/data/pellcorp/k1/config-helper.py --add-include "SimpleAddon/quickstart.cfg"
```


# Auto Save Z Offset
Auto Save Z Offset - Automatically saves gcode_z_offset into a variables files each time a change is made and auto loads z_offset on startup.

```
mkdir -p /usr/data/printer_data/config/SimpleAddon
wget -O /usr/data/printer_data/config/SimpleAddon/save-zoffset.cfg https://raw.githubusercontent.com/ZeroDotCMD/SimpleAddon/main/SimpleAddon/save-zoffset.cfg
/usr/data/pellcorp/k1/config-helper.py --add-include "SimpleAddon/save-zoffset.cfg"
```


