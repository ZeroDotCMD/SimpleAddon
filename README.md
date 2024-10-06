# SimpleAddon for SimpleAF
SimpleAddon adds a few extra helpful options for SimpleAF. Included addons are listed bellow


Auto Save Z Offset - Automatically saves gcode_z_offset into a variables files each time a change is made and auto loads z_offset on startup.

Probe calibration - Dialog window for easier probe setup

Quick Start - Automate basic printer calibration




# Install
SSH into your printer and copy and run the command that matches your probe.



# SimpleAddon for BTT Eddy

```
mkdir -p /usr/data/printer_data/config/SimpleAddon
wget -O /usr/data/printer_data/config/SimpleAddon/eddycalibrate.cfg https://raw.githubusercontent.com/ZeroDotCMD/SimpleAddon/main/SimpleAddon/eddycalibrate.cfg
wget -O /usr/data/printer_data/config/SimpleAddon/quickstart.cfg https://raw.githubusercontent.com/ZeroDotCMD/SimpleAddon/main/SimpleAddon/quickstart.cfg
wget -O /usr/data/printer_data/config/SimpleAddon/save-zoffset.cfg https://raw.githubusercontent.com/ZeroDotCMD/SimpleAddon/main/SimpleAddon/save-zoffset.cfg
echo -e "\n\n[temperature_probe btt_eddy]\nsensor_type: Generic 3950\nsensor_pin: eddy: gpio26\nhorizontal_move_z: 2" >> /usr/data/printer_data/config/btteddy.cfg
/usr/data/pellcorp/k1/config-helper.py --add-include "SimpleAddon/quickstart.cfg"
/usr/data/pellcorp/k1/config-helper.py --add-include "SimpleAddon/eddycalibrate.cfg"
/usr/data/pellcorp/k1/config-helper.py --add-include "SimpleAddon/save-zoffset.cfg"
```


