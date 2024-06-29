### For Linux UBUNTU +16 :

Go to the Directory 
``` /etc/netplan/ ```

Use [this file](00-installer-config-DHCP-Network-Type-ubuntu+16.yaml)

Notice That After modifying config file Run :
```netplan apply```


### For Linux UBUNTU <=16 :

Go to the Directory 
``` /etc/network/ ```

Open ``` interfaces ``` via nano or vi

Use [this file](interfaces)

Notice That After modifying config file Run :

```systemctl restart networking```

### For Linux CentOS 7 :

Go to the Directory 
```/etc/sysconfig/network-scripts/ ```

Open ``` ifcfg-e-* ``` via  vi

Use [this file](ifcfg-ens33)

Notice That After modifying config file Run :

```systemctl restart network```

**For Generate New UUID For [New Network card]:

uuidgen [New Network card] >> ifcfg-[New Network card]
for example: uuidgen enp0s8 >> ifcfg-enp0s8

||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||

ip a  = ifconfig

ip r   = route -n


