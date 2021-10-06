## Open .bashrc file
```
vi ~/.bashrc
```

## Add below sentences
```
export {variablename}='{wanted path}'
```

## Apply setting
```
source ~/.bashrc
```

## Alternatives
```
sudo update-alternatives --config {command}
sudo update-alternatives --install {target_file_path} {command} {bind_file_path}
```
### example
```
sudo update-alternatives --config python3
sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.9
```
