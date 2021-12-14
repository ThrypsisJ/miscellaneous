# lshw : list hardware
### Use case
* list network devices
```console
user@device:~$ sudo lshw -class network
  *-virtio1                 
       description: Ethernet interface
       physical id: b
       bus info: virtio@1
       logical name: eth0
       serial: 00:00:00:00:00:00
       capabilities: ethernet physical logical
       configuration: autonegotiation=off broadcast=yes driver=virtio_net driverversion=1.0.0 ip=10.211.55.20 link=yes multicast=yes
  *-network DISABLED
       description: Ethernet interface
       physical id: 1
       bus info: usb@3:4
       logical name: enx004ee4ac1ce5
       serial: 00:00:00:00:00:00
       size: 100Mbit/s
       capacity: 1Gbit/s
       capabilities: ethernet physical tp mii 10bt 10bt-fd 100bt 100bt-fd 1000bt 1000bt-fd autonegotiation
       configuration: autonegotiation=on broadcast=yes driver=r8152 driverversion=v1.10.11 duplex=full link=no multicast=yes port=MII speed=100Mbit/s
```
