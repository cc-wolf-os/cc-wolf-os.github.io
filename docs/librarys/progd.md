---
status: new
---

# Progd
!!! danger "progd lib"
    the progd lib is not yet implemented


## Methods
### `.load(<catagory>)`
returns a ProgDB wrapper


## Types
### ProgDB
Propane DB wraper
#### Methods
##### addProgram

```lua
:addProgram(<program name>,<path>,<program char icon>,[args])
```

| Arg               | Description                          |
| ----------------- | ------------------------------------ |
| Program name      | the program's name                   |
| Path              | the path to the program              |
| program char icon | A single char for the program's icon |
| Args (optional)   | any args to pass to the program      |

##### close
```lua
:close()
```
closes and saves any db changes