# SimpleAddon for SimpleAF
SimpleAddon adds a few extra helpful options for SimpleAF. Included addons are listed bellow
<br><br>
Probe calibration - Dialog window for easier probe setup for probes.<br>
Quick Start - Quick Start is a single macro that runs through the basic calibrations required to begin printing, including PID calibration for both the printer's bed and hotend, as well as input shaping.





# Install
SSH into your printer and copy and run the command that matches your probe.
<br><br>

# SimpleAddon for Cartographer 3D

```
mkdir -p /usr/data/printer_data/config/addons
wget -O /usr/data/printer_data/config/addons/cartographer_calibrate.cfg https://raw.githubusercontent.com/ZeroDotCMD/SimpleAddon/main/SimpleAddon/cartographer_calibrate.cfg
wget -O /usr/data/printer_data/config/addons/quickstart.cfg https://raw.githubusercontent.com/ZeroDotCMD/SimpleAddon/main/SimpleAddon/quickstart.cfg
/usr/data/pellcorp/k1/config-helper.py --add-include "addons/*.cfg"
```
<br>

# SimpleAddon for BTT Eddy

```
mkdir -p /usr/data/printer_data/config/addons
wget -O /usr/data/printer_data/config/addons/eddycalibrate.cfg https://raw.githubusercontent.com/ZeroDotCMD/SimpleAddon/main/SimpleAddon/eddycalibrate.cfg
wget -O /usr/data/printer_data/config/addons/eddycalibrate.cfg https://raw.githubusercontent.com/ZeroDotCMD/SimpleAddon/main/SimpleAddon/eddycalibrate.cfg
wget -O /usr/data/printer_data/config/addons/quickstart.cfg https://raw.githubusercontent.com/ZeroDotCMD/SimpleAddon/main/SimpleAddon/quickstart.cfg
/usr/data/pellcorp/k1/config-helper.py --add-include "addons/*.cfg"
```
<br>



