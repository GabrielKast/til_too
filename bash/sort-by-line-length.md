## Sort a file by length of line

Just the kind of snippet I always use and always forget.
```
cat myfile.txt | awk '{ print length, $0 }' | sort -n | cut -d" " -f2-
```
from [that answer on stackoverflow](https://stackoverflow.com/questions/5917576/sort-a-text-file-by-line-length-including-spaces)
