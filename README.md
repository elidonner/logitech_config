# logitech_config
This contains my logitech mouse settings for linux using the opensource logiops.

Follow:
https://github.com/PixlOne/logiops/tree/main

for building the app.

After running `sudo systemcctl enable --now logid`.

Default location is `/etc/logid.cfg` but you can run `sudo logid -c /filepath` to choose a different location. I don't know how to make it do this on system reboot without having default file in `/etc/logid.cfg`.

## How to uninstall

First, disable the daemon:
```bash
sudo systemctl disable --now logid
```

Then remove the few files that were installed:
```bash
sudo rm /usr/local/bin/logid
sudo rm /lib/systemd/system/logid.service
sudo rm /etc/logid.cfg
```


To modify the code:
* Help wiki is [here](https://github.com/PixlOne/logiops/wiki/Configuration).
* Compatible devices are listed [here](https://github.com/PixlOne/logiops/blob/main/TESTED.md).
* Linux input-event-codes are [here](https://github.com/torvalds/linux/blob/master/include/uapi/linux/input-event-codes.h).