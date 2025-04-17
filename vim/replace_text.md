### Replace text at current line
* Replace the first matching text
```vim
:s/old/new/
```

* Replace all matching text
```vim
:s/old/new/g
```

### Replace text within the document
* Replace all matching text (case sensitive)
```vim
:%s/old/new/g
```

* Replace all matching text (case insensitive)
```vim
:%s/old/new/gi
```

* Require confirmation every replace
```vim
:%s/old/new/gc
```
