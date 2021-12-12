# How to create SSH key
1. Move to .ssh folder
```console
user@device:~/$ cd .ssh
```

2. Create key
```console
user@device:~/$ ssh-keygen -t ed25519 -C "your_email@example.com"
```

3. Set path and passphrase
```console
Enter file in which to save the key (/home/user/.ssh/id_ed25519): 
Enter passphrase (empty for no passphrase): 
Enter same passphrase again:
```

4. Check public key
```console
user@device:~/$ cat id_ed25519.pub
```
