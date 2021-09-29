## Basic settings

### Install git

```shell
sudo apt-get install git-core
```

### Check version of git

```shell
git version
```

### Set user information

```shell
git config --global user.email "email address"
git config --global user.name "user name"
```

### Change git commands to colored

```shell
git config --global color.ui "auto"
```

### Create working folder

```shell
sudo mkdir {folder name}
cd {folder name}
```

### Create local git storage

```shell
% at working folder
git init
```
\
## Connect to GitHub

### Regist origin(remote storage)

```shell
sudo git remote add origin {remote address}
```

### Check registered origins

```shell
git remote -v
```

### Remove origin
```shell
git remote remove origin
```

### Add folder and check status

```shell
git add {folder}/
git status
```

### Commit to local storage

```shell
git commit -m "Describe commit contents"
```

## Branch

### Create branch

```shell
git branch {branch_name}
```

### Delete branch
```shell
git branch -d {branch_name}
```

### Move git head to branch

```shell
git checkout {branch_name}
```

### Merge branches
```shell
git checkout {main_branch}
git merge {branch_name}
```

## Check log

```shell
git log --oneline --decorate
```

