### Insert lines to file

```
f = open(mtlFile, 'r')
lines = f.readlines()
f.close()
insertAt = 5
lines.insert(insertAt, newLine)
f = open(mtlFile, 'w')
lines = ''.join(lines) # list to string
f.write(lines)
f.close()
```