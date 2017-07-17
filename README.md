**Warning**: This version is built to run on Docker that is hosted on a Raspberry Pi 3.

All you have to do is to plug in your RTL2832u compatible USB receiver and run the container!

```bash
docker run --privileged -v /dev/bus/usb:/dev/bus/usb seanstaley/rpi-dump1090
```

It exposes the following ports:
 - 8080 -> data feeds and basic website for data visualisation
 - 30001 -> raw input port
 - 30002 -> raw output
 - 30003 -> SBS1 (BaseStation) format output
 - 30004 -> Beast input port
 - 30005 -> Beast output port
