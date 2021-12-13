# Set NTP server on Ubuntu
## Install NTP
```console
user@device:~$ sudo apt install ntp
```

## Modify /etc/ntp.conf
* open /etc/ntp.conf
```console
user@device:~$ sudo vi /etc/ntp.conf
```

* modify configuration
```python
...
# delete
# pool 0.ubuntu.pool.ntp.org iburst
# pool 1.ubuntu.pool.ntp.org iburst
# pool 2.ubuntu.pool.ntp.org iburst
# pool 3.ubuntu.pool.ntp.org iburst
server  127.127.1.0 prefer
fudge   127.127.1.0
...
# security setting
restrict  default
...
# broadcast setting
broadcast 192.168.10.* # for Nerian Scarlet 3D
```
