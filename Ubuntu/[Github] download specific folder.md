# Downloads specific folder
## Activate sparse-checkout option
```
git config core.sparseCheckout true
```

## add remote
```
git remote add -f origin <link>
```

## create sparse-checkout file
```
vi .git/info/sparse-checkout
```

## insert wanted path into sparse-checkout file
```
./Path
```

## pull
```
git pull origin main
```
