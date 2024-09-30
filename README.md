Install quick start macros 
SSH into your printer and run this command to copy Quick Start to your install.

```
wget -O /usr/data/printer_data/config/quickstart.cfg https://raw.githubusercontent.com/ZeroDotCMD/test/main/quickstart.cfg
```

Once the command is run You'll need to add ``` [include quickstart.cfg] ``` to the top of Your printer.cfg
