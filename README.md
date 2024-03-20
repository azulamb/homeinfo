# homeinfo

## Setup


```
sudo raspi-config
```

```
sudo dphys-swapfile swapoff
sudo vim /etc/dphys-swapfile
```

Change `CONF_SWAPSIZE` = `2048`

```
sudo dphys-swapfile setup
sudo dphys-swapfile swapon
```

```
mkdir -p ~/.config/lxsession/LXDE-pi
cp /etc/xdg/lxsession/LXDE-pi/autostart ~/.config/lxsession/LXDE-pi/
echo "/bin/sh /home/USER/homeinfo/script/autostart.sh" >> ~/.config/lxsession/LXDE-pi/autostart
```
