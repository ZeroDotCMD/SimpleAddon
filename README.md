Install quick start macros 
SSH into your printer and run this command to copy Quick Start and Eddy calibration to your install.

```
mkdir -p /usr/data/printer_data/config/simpleaddon
wget -O /usr/data/printer_data/config/simpleaddon/eddycalibrate.cfg https://raw.githubusercontent.com/ZeroDotCMD/test/main/eddycalibrate.cfg
wget -O /usr/data/printer_data/config/simpleaddon/quickstart.cfg https://raw.githubusercontent.com/ZeroDotCMD/test/main/quickstart.cfg
wget -O /usr/data/printer_data/config/simpleaddon/autozoffset.cfg https://raw.githubusercontent.com/ZeroDotCMD/test/main/autozoffset.cfg
sed -i '12i [include simpleaddon/quickstart.cfg]\n\n[include simpleaddon/eddycalibrate.cfg]\n\n[include simpleaddon/autozoffset.cfg]' /usr/data/printer_data/config/printer.cfg

```


