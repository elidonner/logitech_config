# logitech_config
This contains my logitech mouse settings for linux using the opensource logiops.

Follow:
https://github.com/PixlOne/logiops/tree/main

for building the app.

After running `sudo systemcctl enable --now logid`, you can run `sudo logid` to enable the config file. Default location is `/etc/logid.cfg` but you can run `sudo logid -c /filepath` to choose a different location.


To modify the code:
* Help wiki is [here](https://github.com/PixlOne/logiops/wiki/Configuration).
* Compatible devices are listed [here](https://github.com/PixlOne/logiops/blob/main/TESTED.md).
* Linux input-event-codes are [here](https://github.com/torvalds/linux/blob/master/include/uapi/linux/input-event-codes.h).