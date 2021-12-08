# Samba server setting
## install Samba
```console
user@desktop:~$ sudo apt-get install samba
```

## modify configuration
* open Samba configuration file
```console
user@desktop:~$ sudo vi /etc/samba/smb.conf
```

* samba port setting
```ini
[global]
...
# Add
smb ports = port1, port2
...

...
# Add
[share_name]
   comment = share_name
   path = share_path
   read_only = no
   browsable = yes
   valid users = user_name
```

* add user and restart samba
```console
user@desktop:~$ sudo smbpasswd -a user_name
user@desktop:~$ sudo service smbd restart
```
