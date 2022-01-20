### Clear page cache only
```bash
sudo sh -c 'echo 1 >  /proc/sys/vm/drop_caches'
```

### Clear dentries and inodes
```bash
sudo sh -C 'echo 2 >  /proc/sys/vm/drop_cahces'
```

### Clear PageCache, dentries and inodes
```bash
sudo sh -c 'echo 3 >  /proc/sys/vm/drop_caches'
```
